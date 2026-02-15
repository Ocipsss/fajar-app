<script setup>
import SplitScreen from './components/layout/SplitScreen.vue';
import { ref } from 'vue';

const mockSupplier = ref("PT. Sumber Rejeki");
</script>

<template>
  <SplitScreen>
    <template #top>
      <div class="w-full h-full flex items-center justify-center text-gray-500">
        <div class="text-center">
          <div class="mb-2 text-4xl">📸</div>
          <p class="text-xs uppercase tracking-widest font-semibold text-gray-400">Camera Preview</p>
        </div>
      </div>
    </template>

    <template #bottom>
      <div class="space-y-6">
        <header class="flex justify-between items-end">
          <div>
            <h1 class="text-2xl font-bold text-gray-800">Entry Struk</h1>
            <p class="text-sm text-gray-500">{{ mockSupplier }}</p>
          </div>
          <span class="text-xs font-mono bg-gray-200 px-2 py-1 rounded text-gray-600">
            v0.1-Alpha
          </span>
        </header>

        <div class="space-y-4">
          <div class="p-4 bg-white rounded-2xl border border-gray-100 shadow-sm">
            <p class="text-gray-400 text-sm italic">Menunggu input barang...</p>
          </div>
        </div>
      </div>
    </template>
  </SplitScreen>
</template>