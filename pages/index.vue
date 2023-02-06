<template>

  <div>
    <!--  表頭  -->
    <div class="fixed flex row bg-accent w-screen h-16 ">
      <p class="basis-4/6 text-white h-full text-justify">Matcha Note</p>
      <p class="basis-1/6 text-white">登入</p>
      <p class="basis-1/6 text-white">登入</p>

    </div>
    <!--  Pager Header  -->
    <div class="static top-16 fixed flex bg-warning w-screen h-16">

    </div>


    <!--  Page Content  -->
    <div class="overflow-auto pt-32 pb-24 h-screen w-screen bg-gray-400 ">

      <div v-for="item in state.for" class="h-24 w-screen bg-red-600 my-6">
        {{ item }}
      </div>

    </div>

    <!--  Navigation Bottom Bar  -->
    <div class="fixed row bottom-0 right-0 flex row bg-accent w-screen h-24">
      <div class="basis-1/2">首頁</div>
      <div class="basis-1/2">茶道知識</div>
    </div>

  </div>

</template>

<script setup lang="ts">

const state = reactive({
  for: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
})

</script>