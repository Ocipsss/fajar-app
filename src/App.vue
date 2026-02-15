<template>
  <div class="h-screen flex flex-col overflow-hidden bg-gray-100">
    <div class="h-1/2 bg-black relative flex items-center justify-center border-b-2 border-orange-500">
      <div class="absolute top-4 left-4 z-10">
        <span class="bg-orange-500 text-white px-3 py-1 rounded-full text-xs font-bold shadow-lg">
          PREVIEW STRUK
        </span>
      </div>
      <div class="text-gray-500 text-center">
        <p class="text-sm italic">Belum ada foto struk.</p>
        <button class="mt-2 bg-white text-black px-4 py-2 rounded-lg font-bold">Ambil Foto</button>
      </div>
    </div>

    <div class="h-1/2 overflow-y-auto p-4 space-y-4 pb-20">
      <h2 class="font-bold text-lg text-gray-800">Detail Pembelian</h2>
      
      <div class="bg-white p-4 rounded-xl shadow-sm border border-gray-200">
        <label class="block text-xs font-bold text-gray-500 uppercase">Nama Barang / SKU</label>
        <input type="text" class="w-full border-b-2 border-gray-300 py-2 focus:border-orange-500 outline-none transition-colors" placeholder="Ketik nama atau alias...">
      </div>

      <div class="grid grid-cols-2 gap-4">
        <div class="bg-white p-4 rounded-xl shadow-sm border border-gray-200">
          <label class="block text-xs font-bold text-gray-500 uppercase">Qty (Dus/Pcs)</label>
          <input type="number" class="w-full border-b-2 border-gray-300 py-2 focus:border-orange-500 outline-none" placeholder="0">
        </div>
        <div class="bg-white p-4 rounded-xl shadow-sm border border-gray-200">
          <label class="block text-xs font-bold text-gray-500 uppercase">Harga Total</label>
          <input type="number" class="w-full border-b-2 border-gray-300 py-2 focus:border-orange-500 outline-none" placeholder="Rp 0">
        </div>
      </div>
    </div>

    <button class="fixed bottom-6 right-6 bg-orange-600 text-white w-14 h-14 rounded-full shadow-2xl flex items-center justify-center text-2xl font-bold">
      +
    </button>
  </div>
</template>

<script setup>
// Nanti logika database masuk sini
</script>