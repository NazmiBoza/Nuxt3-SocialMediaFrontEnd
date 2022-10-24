<template>
    <div>
        <div v-for="a in 5">
            <div class="flex mt-2 mb-2 ml-2 mr-2">
                        <div class="alert-img">
                            <img src="/images/person.jpg" class="h-12 w-12 rounded-full" alt="">
                        </div>
                        <div class="alert-info">
                            <p class="text-sm theme-color-text">Nazmi Boza</p>
                            <p class="text-xs theme-color-text">Paylaşımında seni etiketledi.</p>
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