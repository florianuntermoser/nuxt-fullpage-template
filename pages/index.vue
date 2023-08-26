<template>
  <div class="snap-y snap-mandatory h-screen overflow-y-scroll">
    <section class="snap-center snap-always h-full justify-center bg-black/10">
      <FadeOnIntersection class="h-full w-full flex items-center justify-center">Section 1</FadeOnIntersection>
    </section>
    <section class="snap-center snap-always h-full justify-center">
      <FadeOnIntersection class="h-full w-full flex items-center justify-center">Section 2</FadeOnIntersection>
    </section>
    <section class="snap-center snap-always h-full justify-center bg-black/10">
      <FadeOnIntersection class="h-full w-full flex items-center justify-center">Section 3</FadeOnIntersection>
    </section>
  </div>
</template>