<template>
<div :class="[`border-infoblue`]" class="bg-infoblue dark:bg-tokyosky border-2 text-white p-4 my-8 infobox overflow-hidden shadow-sm rounded-lg twitter-cta cvis">
  <p class="m-0 text-white text-sm md:text-2xl text-center text-base">Enjoyed the article? Consider <a target="_blank" rel="noopener nofollow" :href="shareLink" class="text-retroyellow dark:text-retrogreen dark:green-glow">sharing</a> on <span class="text-retroteal dark:teal-glow">Twitter</span>!</p>
</div>
</template>

<script>
export default {
  props: ['shareLink']
}
</script>

<style scoped>
.dark .twitter-cta {
  filter: drop-shadow(0px 0px 15px rgba(47,64,235,0.6));
}

.light .twitter-cta a {
  text-shadow: none !important;
}
</style>