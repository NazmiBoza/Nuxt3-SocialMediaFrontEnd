<template>
    <div class="theme-color h-[30rem] w-5/12 rounded-[2%] flex flex-col items-center">
        <p class="text-xl theme-color-text self-center mt-4"><b>Hikayeler</b></p>
        <div class="flex flex-col">
            <div class="story flex items-center ml-4 mt-4 ">
                <div class="flex circle rounded-full border-4 border-green-700 border-dotted w-16 h-16 justify-center items-center">
                    <img class=" w-8 h-8 opacity-70 theme-icon" src="/icons/plus.svg" alt="">
                </div>
                    
                    <div class="ml-4">
                        <p class="theme-color-text">Yeni bir hikaye ekle</p>
                        <p class="theme-color-text text-xs">Bir anını veya fotoğrafını paylaş...</p>
                    </div>
                </div>
           
                <div class="story flex ml-4 mt-4">
                    <img class="rounded-full w-16 h-16 border-4 border-green-700 border-dotted" src="/images/person.jpg" alt="">
                    <div class="ml-4">
                        <p class="theme-color-text mt-2">Nazmi Boza</p>
                        <p class="theme-color-text">5 Saat Önce</p>
                    </div>
                </div>
                <div class="story flex ml-4 mt-4">
                    <img class="rounded-full w-16 h-16 border-4 border-green-700 border-dotted" src="/images/person.jpg" alt="">
                    <div class="ml-4">
                        <p class="theme-color-text mt-2">Nazmi Boza</p>
                        <p class="theme-color-text">5 Saat Önce</p>
                    </div>
                </div>
                <div class="story flex ml-4 mt-4">
                    <img class="rounded-full w-16 h-16 border-4 border-green-700 border-dotted" src="/images/person.jpg" alt="">
                    <div class="ml-4">
                        <p class="theme-color-text mt-2">Nazmi Boza</p>
                        <p class="theme-color-text">5 Saat Önce</p>
                    </div>
                </div>
                <div class="story flex ml-4 mt-4">
                    <img class="rounded-full w-16 h-16 border-4 border-green-700 border-dotted" src="/images/person.jpg" alt="">
                    <div class="ml-4">
                        <p class="theme-color-text mt-2">Nazmi Boza</p>
                        <p class="theme-color-text">5 Saat Önce</p>
                    </div>
                </div>
                
        </div>
        
     </div>
</template>

<style>
.theme-color{
    background-color: #082032;
}
.theme-color-light{
    background-color: #334756;
}
.theme-color-text{
    color:white;
}
.theme-icon{
    filter: invert(0);
}
</style>