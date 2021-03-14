<template>
  <div class="">
    <span class="font-semibold text-gray-700">🏆 Top 10 콘텐츠</span>
  </div>
  <div class="flex py-4 overflow-x-scroll">
    <div class="w-full" v-for="i in Array(10)" :key="i">
      <card />
    </div>
  </div>
</template>

<script>
import Card from "./Card.vue";
export default {
  components: { Card },
};
</script>
