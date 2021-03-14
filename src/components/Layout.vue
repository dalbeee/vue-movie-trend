<template>
  <div class="flex justify-center bg-gray-50">
    <div class="w-full min-h-screen">
      <Header />
      <content />
    </div>
  </div>
</template>

<script>
import Content from "./Content.vue";
import Header from "./Header.vue";

export default {
  components: {
    Header,
    Content,
  },
};
</script>

<style></style>
