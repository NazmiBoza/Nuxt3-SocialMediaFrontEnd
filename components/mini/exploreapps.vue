<template>
    <div class="flex justify-center items-center">
        <div class="mt-16 grid grid-cols-3 gap-8 auto-cols-fr w-8/12">

        <div v-for="n in 9">
            <div class="app flex flex-col items-center">
            <div class="icon">
                <img class="w-36" src="/icons/shop.svg" alt="">
            </div>
            <div class="text text-2xl theme-color-text">Market</div>
            </div>
        </div>
    </div>
    
    </div>
</template>

<style>
.theme-color-text{
    color:white;
}
</style>