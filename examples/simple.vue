<template>
  <div>
    <h2>Simple</h2>
    <vue-horizontal-list-autoscroll :items="items" :options="options">
      <template v-slot:default="{ item }">
        <div class="item">
          <h3>{{ item.title }}</h3>
          <p>{{ item.content }}</p>
        </div>
      </template>
    </vue-horizontal-list-autoscroll>
  </div>
</template>

<script>
import VueHorizontalListAutoscroll from "@/vue-horizontal-list-autoscroll.vue";

export default {
  name: "simple",
  components: {
    VueHorizontalListAutoscroll,
  },
  data() {
    return {
      items: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9].map((i) => {
        return { title: `Item ${i}`, content: `🚀 Simple content ${i}` };
      }),
      options: {},
    };
  },
};
</script>

<style scoped>
.item {
  padding: 16px 24px;
  border-radius: 3px;
  background: #f5f5f5;
}
</style>
