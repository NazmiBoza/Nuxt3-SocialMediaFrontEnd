<script setup>
function onfocusin(){
    
    document.getElementById("publish").style.height="18rem";
}
function onfocusout(){
   console.log(document.getElementById("text").value)
    if (document.getElementById("text").value ==""){
        
        document.getElementById("publish").style.height="8rem";
    }
    else{
        document.getElementById("publish").style.height="18rem";
    }
}


 
</script>

<template>
    
    <div id="publish" class="theme-color h-32 rounded-[1.5%] flex flex-col transition-all duration-700 w-full">
        <div class="flex basis-11/12">
            <div class="left-4 top-3">
            <img class="w-12  rounded-full md:ml-2 mt-2" src="/images/person.jpg" alt="">
    </div>
     <textarea id="text" @focusin="onfocusin" @focusout="onfocusout" class="resize-none  mt-2 mb-2 md:mr-2 md:ml-4 rounded-lg focus:outline-none theme-color theme-color-text" 
     type="text" placeholder="Günün Nasıl Geçti..."></textarea>
    </div>
    
     <div class="buttons basis-1/12 flex justify-center">
      
        
        <div class="pushbutton theme-color-light md:ml-4">
            <input type="file" class="opacity-0 absolute md:left-[41%] left-[5%] w-24" accept="image/*" @change="onChange" />
            <img class="w-6 h-6 mr-2 theme-icons" src="/icons/media.svg" alt="">
            <p class="theme-color-text">Medya</p>
        </div>
        
        
        <a href="#">
        <div class="pushbutton theme-color-light md:ml-4">
            <img class="w-6 h-6 mr-2 theme-icons" src="/icons/activity.svg" alt="">
            <p class="theme-color-text">Aktivite</p>
        </div>
        </a>

        <a href="#">
        <div class="pushbutton theme-color-light md:ml-4">
            <img class="w-6 h-6 mr-2 theme-icons" src="/icons/emotion.svg" alt="">
            <p class="theme-color-text">Duygu</p>
        </div>
        </a>
     </div>
</div>   
   
</template>

<style>
.pushbutton{
    display: flex;
    align-items: center;
    justify-content: center;   
    width: 8rem;
    height: 2.5rem;
    border-radius: 5% 5% 0 0;
}
.theme-color{
    background-color: #082032;
}
.theme-color-light{
    background-color: #334756;
}
.theme-color-text{
    color:white;
}
.theme-icons{
    filter: invert(0%);
}
</style>