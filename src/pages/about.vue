<template>
  <div>
    <About />
    <Brands />
    <div class="flex justify-between mb-[40px] container">
      <p class="font-bold text-[30px] md:text-[40px] leading-[54.64px]">Блог</p>
      <router-link
        to="/blog"
        class="md:flex hidden items-center border border-[#454545] py-[14px] px-[48px] rounded-[100px] gap-3"
      >
        <p class="font-medium text-[16px] leading-[21.86px]">Перейти в блог</p>
        <img src="/strelka.png" alt="Arrow" />
      </router-link>
    </div>

    <Blog />

    <router-link
      to="/blog"
      class="container mb-[30px] flex md:hidden items-center border border-[#454545] py-[14px] px-[48px] rounded-[100px] gap-3 justify-center"
    >
      <p class="font-medium text-[16px] leading-[21.86px]">Перейти в блог</p>
      <img src="/strelka.png" alt="Arrow" />
    </router-link>
  </div>
</template>

<script setup>
import About from "../components/about/About.vue";
import Brands from "../components/home/brands.vue";
import Blog from "../components/home/blog.vue";
</script>

<style lang="scss" scoped></style>
