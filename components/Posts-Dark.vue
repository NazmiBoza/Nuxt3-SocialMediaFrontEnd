<template>
    <div class="max-w-full">

    
    <div class="theme-color h-auto max-w-full mt-2 rounded-[1.5%] flex flex-col">
       <div class="flex justify-between">
        <div class="pub-left flex">
            <div class="person flex items-center md:gap-3 w-full">
        <img class="w-12 rounded-full md:ml-2 mt-2" src="/images/person.jpg" alt="">
        <div class="flex flex-col ">
            <p class="theme-color-text text-lg">Nazmi Boza</p>
            <p class="theme-color-text text-xs">Yayınlanma Tarihi : 04-04-2023</p> 
        </div>
    </div>
    </div>
        <div class="pub-right">
           <a href=""><img class="w-8 h-8 md:mr-4 mt-4 rotate-90 theme-icons" src="/icons/more.svg" alt=""></a> 
        </div>
       
        
            
        </div>
    <div class="text"><p class="theme-color-text md:mr-4 md:ml-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer aliquet ligula vitae finibus aliquet. 
        Vivamus ipsum lorem, tincidunt sed elementum ac, tempus vel ex. Duis suscipit vestibulum nibh, in porta urna molestie ac. 
        Morbi sit amet ex in lorem fermentum pulvinar. Ut sollicitudin posuere justo vitae vulputate. Vestibulum viverra at nunc ut ultricies.
        Donec vitae augue vehicula</p></div>

       <div class="photo flex md:justify-center"><img class="mt-2 md:mr-4 md:ml-4 rounded-xl" src="/images/publish-1.jpg" alt="">
        <div class="reaction h-12 absolute mt-[65%] ml-[50%] md:mt-[17.5%] md:ml-[19%] flex gap-4">
            <button class="icon-button">
                <img class="h-6 theme-icons" src="/icons/comment.svg" alt="">
            </button>
            <button class="icon-button">
                <img class="h-6 theme-icons" src="/icons/heart.svg" alt="">
            </button>
            <button class="icon-button">
                <img class="h-6 theme-icons" src="/icons/link.svg" alt="">
            </button>
        </div>
       

    </div>

       <div class="reactions h-10 flex items-center">
        <div class="people-icons flex ml-4 -space-x-4">
        <img class="w-8 h-8 rounded-full  mt-2" src="/images/person.jpg" alt="">
        <img class="w-8 h-8 rounded-full  mt-2" src="/images/person.jpg" alt="">
        <img class="w-8 h-8 rounded-full  mt-2" src="/images/person.jpg" alt=""></div>
        <p class="theme-color-text ml-2 text-xs">Nazmi, Ahmet ve daha fazlası bu gönderiyi beğendi</p>
       </div>

</div>   
</div>
</template>

<style>
.icon-button{
    display: flex;
    align-items: center;
    justify-content: center;   
    width: 2.5rem;
    height: 2.5rem;
    border-radius: 100%;
    background-color: #5F9DF7;
}
.icon-button:hover{
    background-color: #FF4C29;
    transition: background-color 0.3s;
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