<script setup>

function onXclick(){
    document.getElementById("alertBox").style.display="none";
}
</script>
<template>
<div id="alertBox" class="flex bg-red-200 text-black font-semibold p-4 text-sm rounded border border-red-300 my-3">
    <div class="flex-grow">Arayüz Halen Geliştirilme Aşamasındadır. <br> Bolca Hata bulunmaktadır!</div>
    <div @click="onXclick" class="flex-shrink cursor-pointer text-red-600 hover:text-red-800" aria-label="Close">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"></path>
        </svg>
    </div>
</div>
</template>