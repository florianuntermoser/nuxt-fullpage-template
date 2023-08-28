<template>
  <div class="snap-y snap-mandatory h-screen overflow-y-scroll">
    <section class="snap-center snap-always h-full justify-center bg-black/10">
      <FadeOnIntersection class="h-full w-full">
        <div class="fixed inset-0 pointer-events-none	flex items-center justify-center">
          <div class="pointer-events-auto">
            Section 1
            <button>Test 1</button>
          </div>
        </div>
      </FadeOnIntersection>
    </section>
    <section class="snap-center snap-always h-full justify-center">
      <FadeOnIntersection class="h-full w-full">
        <div class="fixed inset-0 pointer-events-none	flex items-center justify-center">
          <div class="pointer-events-auto">
            Section 2
            <button>Test 2</button>
          </div>
        </div>
      </FadeOnIntersection>
    </section>
    <section class="snap-center snap-always h-full justify-center bg-black/10">
      <FadeOnIntersection class="h-full w-full">
        <div class="fixed inset-0 pointer-events-none	flex items-center justify-center">
          <div class="pointer-events-auto">
            Section 3
            <button>Test 3</button>
          </div>
        </div>
      </FadeOnIntersection>
    </section>
  </div>
</template>