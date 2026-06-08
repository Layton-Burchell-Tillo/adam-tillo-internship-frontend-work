<script lang="ts" setup>
defineProps<{
  imgUrl: string;
  brandName: string;
  discount: number;
}>();
</script>

<template>
  <div
    class="bg-[#393656] p-7 text-white flex gap-4 flex-col rounded-3xl border border-white/20 h-[270px] w-[270px]"
  >
    <img
      :src="$props.imgUrl"
      class="rounded-2xl max-w-[300px] max-h-[160px] aspect-[30_16]"
    />
    <div class="flex flex-col gap-2">
      <h1 class="font-medium">{{ $props.brandName }}</h1>
      <span>{{ $props.discount }}%</span>
    </div>
  </div>
</template>
