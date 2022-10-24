<template>
    <div>
        <div v-for="a in 5">
            <div class="flex items-center mt-2 ml-2 mr-2 mb-2">
                        <div class="chat-img">
                            <img src="/images/person.jpg" class="h-12 w-12 rounded-full" alt="">
                        </div>
                        <div class="chat-info w-36">
                            <p class="text-sm theme-color-text">Nazmi Boza</p>
                            <p class="text-xs theme-color-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit... </p>
                        </div>
                        <div class="chat-icon mr-4 mt-2 w-8 h-8">
                            <img src="/icons/chat.svg" class="h-8 w-8" alt="">
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