<template>
  <UContainer class="my-8" :ui="{ constrained: 'max-w-screen' }">
    <div class="flex flex-col items-center justify-center gap-4 md:gap-8">
      <div class="font-bold">
        <p class="text-center text-xl md:text-6xl">One people come form ALL</p>
        <CommonBrandText
          label="parts of startup ecosystem"
          class="text-center text-xl md:text-6xl"
          color="blue-700"
          background
          slide
        />
      </div>
      <p class="mb-4 text-center text-xs md:text-base">
        Our leadership, members, and alumni work in VCs and startups, just like
        you. We're young, closely connected, and understand young founders.
      </p>
    </div>
    <div class="mx-auto mt-4 flex w-fit flex-col gap-4 lg:flex-row">
      <HomepageMemberIntroItem
        v-for="item in items"
        :key="item.text"
        :places="item.places"
        :text="item.text"
      />
    </div>
  </UContainer>
</template>

<script setup lang="ts">
const items = ref([
  {
    text: 'We live in',
    places: [
      '/countries/live/Canada.png',
      '/countries/live/Czech.png',
      '/countries/live/Finland.png',
      '/countries/live/Hungary.png',
      '/countries/live/Korea.png',
      '/countries/live/Netherlands.png',
      '/countries/live/Vietnam.png',
      '/countries/live/America.png',
      '/countries/live/Australia.png'
    ]
  },
  {
    text: 'We study at',
    places: [
      '/countries/study/FTU.png',
      '/countries/study/FullBright.png',
      '/countries/study/NYU.png',
      '/countries/study/BUV.png',
      '/countries/study/Cornell.png',
      '/countries/study/Frame 1263.png',
      '/countries/study/Frame 1264.png',
      '/countries/study/Frame 1265.png'
    ]
  },
  {
    text: 'We work at',
    places: [
      '/countries/work/Ericsson.png',
      '/countries/work/Frame 1266.png',
      '/countries/work/Genesia Ventures.png',
      '/countries/work/GIMO.png',
      '/countries/work/Masan.png',
      '/countries/work/McKinsey.png',
      '/countries/work/MOMO.png',
      '/countries/work/Nielsen IQ.png',
      '/countries/work/Starbucks.png',
      '/countries/work/Think Zone.png',
      '/countries/work/BCG.png',
      '/countries/work/Dentons.png'
    ]
  }
])
</script>
