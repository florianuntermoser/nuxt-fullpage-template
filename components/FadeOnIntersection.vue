<template>
  <div class="intersectionElement" ref="intersectionDiv">
    <slot />
  </div>
</template>
<script setup>
const intersectionDiv = ref(null)

onMounted(() => {
  if (!intersectionDiv.value) {
    return
  }
  
  const intersectFadingItemsObserver = new IntersectionObserver((entries) => {
    for (const entry of entries) {
      const element = entry.target

      element.setAttribute("style", `--intersection-opacity: ${entry.intersectionRatio.toFixed(2)}`)
    }
  }, {
    threshold: [...Array(100).keys()].map(k => k / 100.0)
  });
  // start observing
  intersectFadingItemsObserver.observe(intersectionDiv.value);
})
</script>
<style scoped>
.intersectionElement {
  --intersection-opacity: 0;
}
.intersectionElement {
  opacity: var(--intersection-opacity);
}
</style>