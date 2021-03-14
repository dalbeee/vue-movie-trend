<template>
  <div class="flex justify-center py-4">
    <div class="w-11/12">
      <!-- top 10 -->
      <div class="w-full">
        <top-ten />
        <recommand-system />
      </div>
    </div>
  </div>
</template>

<script>
import RecommandSystem from "./RecommandSystem.vue";
import TopTen from "./TopTen.vue";

export default {
  components: { RecommandSystem, TopTen },
};
</script>
