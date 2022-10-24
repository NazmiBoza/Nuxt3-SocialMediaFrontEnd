<script setup>

let enabled = false;
let change = false;
function themeChange()
{
   if (!change)
   {
    change=true;
    var blacks = document.getElementsByClassName("theme-color");
        for (var i=0; i < blacks.length; i++)
        {
            blacks[i].style.transition = "all 0s";
            blacks[i].style.backgroundColor = "#FFFBE7";
            blacks[i].style.transition = "all 0.5s";
        }
    var lightblacks = document.getElementsByClassName("theme-color-light");
        for (var i=0; i < lightblacks.length; i++)
        {
            lightblacks[i].style.backgroundColor = "#E0DECA";
        }
    var lighttext = document.getElementsByClassName("theme-color-text");
        for (var i=0; i < lighttext.length; i++)
        {
            lighttext[i].style.color = "black";
        }
    var ticon = document.getElementsByClassName("theme-icon");
        for (var i=0; i < ticon.length; i++)
        {
            ticon[i].style.filter = "invert(1)";
        }    
   }
   else{
    change=false;
    var blacks = document.getElementsByClassName("theme-color");
        for (var i=0; i < blacks.length; i++)
        {
            blacks[i].style.backgroundColor = "#082032";
        }
    var lightblacks = document.getElementsByClassName("theme-color-light");
        for (var i=0; i < lightblacks.length; i++)
        {
            lightblacks[i].style.backgroundColor = "#334756";
        }
    var lighttext = document.getElementsByClassName("theme-color-text");
        for (var i=0; i < lighttext.length; i++)
        {
            lighttext[i].style.color = "white";
        }
    var ticon = document.getElementsByClassName("theme-icon");
        for (var i=0; i < ticon.length; i++)
        {
            ticon[i].style.filter = "invert(0)";
        }  
    }
 
        
}
</script>
<template>
    <div>
        <div class="flex flex-col">
            <div class="flex justify-evenly items-center theme-color-text">
                <p><b>Nazmi Boza</b></p>
                <label for="AcceptConditions" class="relative h-8 w-14 cursor-pointer">
                <input @change="themeChange" type="checkbox" id="AcceptConditions" class="peer sr-only" />
                <span
                class="absolute inset-0 rounded-full bg-[#334756] transition peer-checked:bg-slate-300"
                ></span>
                <span
                class="absolute inset-0 m-1 h-6 w-6 rounded-full bg-white transition peer-checked:translate-x-6"
                ></span>
                </label>
            </div>
            <div class="flex-grow border-t h-px mt-4 mb-1 opacity-20 ml-4 mr-4"></div>
            <div class="pages flex flex-col">
                <p class="self-center theme-color-text">Sayfalarınız</p>
                <div class="flex mt-2 mb-2 ml-2 mr-2">
                        <div class="pages-img">
                            <img src="/images/person.jpg" class="h-12 w-12 rounded-full" alt="">
                        </div>
                        <div class="pages-info">
                            <p class="text-sm theme-color-text">Kedi Sevenler Derneği</p>
                            <p class="text-xs theme-color-text">Paylaşımında seni etiketledi.</p>
                        </div>
                    </div>
                    <div class="flex mt-2 mb-2 ml-2 mr-2">
                        <div class="pages-img">
                            <img src="/images/person.jpg" class="h-12 w-12 rounded-full" alt="">
                        </div>
                        <div class="pages-info">
                            <p class="text-sm theme-color-text">Kedi Sevenler Derneği</p>
                            <p class="text-xs theme-color-text">Paylaşımında seni etiketledi.</p>
                        </div>
                    </div>
                    <div class="flex items-center justify-center">
                        <p class="theme-color-text">Daha fazla Sayfa...</p>
                    </div>
                    
            </div>
                <div class="flex-grow border-t h-px mt-4 mb-1 opacity-20 ml-4 mr-4 theme-icon"></div>
            <div class="flex mt-2 mb-2 ml-8 mr-2 ">
                        <div class="settings-img">
                            <img src="/icons/settings.svg" class="h-8 w-8 theme-icon" alt="">
                        </div>
                        <div class="settings-info flex items-center">
                            <p class="text-xl theme-color-text ml-2">Ayarlarınız</p>
                            
                        </div>
                    </div>
            <div class="flex mt-2 mb-2 ml-8 mr-2 ">
                        <div class="settings-img">
                            <img src="/icons/settings.svg" class="h-8 w-8 theme-icon" alt="">
                        </div>
                        <div class="settings-info flex items-center">
                            <p class="text-xl theme-color-text ml-2">Yardım</p>
                            
                        </div>
                    </div>
            <div class="flex mt-2 mb-2 ml-8 mr-2 ">
                        <div class="settings-img">
                            <img src="/icons/settings.svg" class="h-8 w-8 theme-icon" alt="">
                        </div>
                        <div class="settings-info flex items-center">
                            <p class="text-xl theme-color-text ml-2">Çıkış Yap</p>
                            
                        </div>
                    </div>

            
        </div>
    </div>
</template>
<style>
.theme-color-text{
    color:white;
}
.theme-icon{
    filter: invert(0);
}
</style>