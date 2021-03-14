<template>
  <div class="pt-12">
    <span class="font-semibold text-gray-700"
      >Bert 모델을 이용한 사용자 기반 추천 시스템</span
    >
    <div class="flex flex-col justify-center pt-2">
      <!-- 좋아하는 장르 -->
      <div class="flex flex-col items-center justify-center">
        <span class="block py-2 font-semibold text-gray-700"
          >좋아하는 장르를 선택해 주세요 ! ❤</span
        >
        <div class="flex">
          <button
            class="p-2 mr-4 text-xl text-gray-700 bg-gray-300 rounded-xl"
            v-for="genre in genres"
            :key="genre.type"
          >
            {{ genre.name }}
          </button>
        </div>
      </div>

      <!-- 즐겨 본 영화 -->
      <div class="flex flex-col items-center justify-center pt-6">
        <span class="block py-2 font-semibold text-gray-700"
          >즐겨 본 영화가 있다면 선택해 주세요! 😊</span
        >
        <div class="flex flex-wrap justify-center">
          <div class="" v-for="i in Array(8)" :key="i">
            <card />
          </div>
        </div>
      </div>

      <!-- 여기 당신이 좋아할 영화 -->
      <div class="flex flex-col items-center justify-center pt-6">
        <span class="font-semibold text-gray-700"
          >여기 당신이 좋아 할 만한 영화를 골라봤어요</span
        >
        <div class="flex flex-wrap justify-center">
          <div class="" v-for="i in Array(3)" :key="i">
            <div class="w-40 h-40 m-4 bg-gray-400 rounded-xl"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { genres } from "../data/data";
import Card from "./Card.vue";

export default {
  data: () => ({
    genres,
  }),

  components: { Card },
};
</script>

<style></style>
