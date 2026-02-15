<template>
  <div class="h-screen w-full flex flex-col overflow-hidden bg-gray-900">
    <div class="relative flex-none h-[45vh] bg-black shadow-xl z-10">
      <slot name="top"></slot>
      
      <div class="absolute top-4 left-4 pointer-events-none">
        <span class="bg-orange-600/80 backdrop-blur-md text-white text-[10px] font-bold px-2 py-1 rounded uppercase tracking-wider">
          Visual Monitor
        </span>
      </div>
    </div>

    <div class="flex-1 bg-gray-50 rounded-t-3xl -mt-6 z-20 overflow-y-auto shadow-[0_-10px_20px_rgba(0,0,0,0.1)]">
      <div class="w-full flex justify-center pt-3 pb-1">
        <div class="w-12 h-1.5 bg-gray-300 rounded-full"></div>
      </div>
      
      <div class="p-5 pb-24">
        <slot name="bottom"></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Memastikan scroll halus di iOS */
.overflow-y-auto {
  -webkit-overflow-scrolling: touch;
}
</style>