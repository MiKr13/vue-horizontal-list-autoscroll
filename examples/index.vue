<template>
  <div id="app">
    <h1>Vue Horizontal List Autoscroll</h1>
    <p>
      You can find all examples here
      <a
        href="https://github.com/mikr13/vue-horizontal-list-autoscroll/tree/master/examples"
        target="_blank"
        >in this folder</a
      >.
    </p>
    <p style="font-style: italic">
      <a
        href="https://www.npmjs.com/package/vue-horizontal-list-autoscroll"
        target="_blank"
        >npm link</a
      >.
    </p>

    <simple />

    <full-width />

    <responsive />

    <auto-scroll />

    <slide-show />

    <image-two />

    <image-three />

    <image-four />

    <image-five />

    <nav-prev-next-slot />

    <item-customization />
  </div>
</template>

<script>
import Vue from "vue";
import VueHorizontalListAutoscroll from "@/vue-horizontal-list-autoscroll.vue";
import Simple from "./simple";
import FullWidth from "./full-width";
import Responsive from "./responsive";
import ItemCustomization from "./item-customization";
import AutoScroll from "./auto-scroll";
import NavPrevNextSlot from "./nav-prev-next-slot";
import ImageTwo from "./image-two";
import ImageThree from "./image-three";
import ImageFour from "./image-four";
import ImageFive from "./image-five";
import SlideShow from "./slide-show";

export default Vue.extend({
  name: "Index",
  components: {
    ImageFive,
    ImageFour,
    ImageThree,
    ImageTwo,
    NavPrevNextSlot,
    AutoScroll,
    ItemCustomization,
    Responsive,
    FullWidth,
    Simple,
    SlideShow,
    VueHorizontalListAutoscroll,
  },
  mounted() {
    document.title = "Vue Horizontal List AutoScroll (MiKr13)";
  },
});
</script>

<style>
body {
  font-family: "-apple-system", "system-ui", "BlinkMacSystemFont", "Segoe UI",
    "Roboto", "Helvetica Neue", "Arial", "sans-serif";
  margin: 0;
  padding: 0;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 0 0 8px;
}

p {
  margin: 0;
  font-size: 17px;
  line-height: 1.5;
  font-weight: 500;
  color: #333;
  word-break: break-word;
}
</style>

<style scoped>
#app {
  max-width: 1400px;

  margin-left: auto;
  margin-right: auto;

  padding: 80px 24px;
}

@media (min-width: 1200px) {
  #app {
    padding-left: 80px;
    padding-right: 80px;
  }
}

#app > div {
  margin: 48px 0;
}
</style>
