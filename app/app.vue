<script setup lang="ts">
const brands = [
  {
    img: "https://cached.imagescaler.hbpl.co.uk/resize/scaleWidth/743/cached.offlinehbpl.hbpl.co.uk/news/OMC/airbnbnewlogo-20140717072746371.jpg",
    name: "Airbnb",
    discount: 7,
  },
  {
    img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5XthyCzw7hiKGKhGSQ3kJtKaSJgWNv0aA-Q&s",
    name: "Aldi",
    discount: 15,
  },
  {
    img: "https://i.ytimg.com/vi/hF8swzNR1-o/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLAB_NX3hz_WksiCr8jrMaRJGk0cZw",
    name: "Apple",
    discount: 10,
  },
  {
    img: "https://static4.franchisedirect.ie/dims4/default/876326e/2147483647/strip/true/crop/350x184+0+18/resize/1200x630!/quality/95/?url=https%3A%2F%2Ffranchisedirect-40-prod-ops.s3.amazonaws.com%2F48%2Fcb%2Fd5cbb2101186078636c8cb6adbfb%2Fburger-king.png",
    name: "Burger King",
    discount: 12,
  },
];
</script>

<template>
  <div class="flex flex-row gap-3 flex-wrap w-full p-4">
    <BrandCard
      v-for="brand in brands"
      :imgUrl="brand.img ?? 'https://placehold.co/300x160'"
      :brandName="brand.name"
      :discount="brand.discount"
    />
  </div>
</template>
