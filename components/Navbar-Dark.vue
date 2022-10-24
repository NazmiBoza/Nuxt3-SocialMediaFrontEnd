<script setup>
import Notifications from './mini/notifications.vue';
import Chats from './mini/chats.vue';
import Exploreapps from './mini/exploreapps.vue';
import PpSettings from './mini/pp-settings.vue';
import { vShow } from 'vue';
let alertbox=false;
let chatbox=false;
let explore=false;
let settings=false;
function AlertOn()
{
    if (!alertbox)
    {
        alertbox=true;
        document.getElementById("alertbox").style.display="flex";
    }
    else{
        alertbox=false;
        document.getElementById("alertbox").style.display="none";
    }

}
function ChatBoxOn()
{
    if (!chatbox)
    {
        chatbox=true;
        document.getElementById("chatbox").style.display="flex";
    }
    else{
        chatbox=false;
        document.getElementById("chatbox").style.display="none";
    }

}

function ExploreBoxOn()
{
    if (!explore)
    {
        explore=true;
        document.getElementById("explore").style.display="flex";
        document.getElementById("explore").style.opacity="100%";
    }
    else{
        explore=false;
        document.getElementById("explore").style.display="none";
        document.getElementById("explore").style.opacity="0%";
    }

}

function SettingsOn()
{
    if (!settings)
    {
        settings=true;
        document.getElementById("pp-settings").style.display="flex";
    }
    else{
        settings=false;
        document.getElementById("pp-settings").style.display="none";
        
    }

}
</script>

<template>
    <div class="navbar-main h-14 theme-color flex items-center justify-between max-w-full" >        
        <div class="nav-left flex">
            <div class="theme-color-text font-bold text-4xl self-center md:ml-4">NB</div>
            <div class="nav-icon md:ml-12 flex items-center md:gap-2">
                <button @click="AlertOn" class="iconbutton">
                    <img class="w-6 h-6 theme-icon" src="/icons/bell.svg" alt="">
                </button>

                <div id="alertbox" class="absolute w-56 rounded-b-lg theme-color top-14 left-[1.6%] flex-col hidden z-10">
                   <Notifications></Notifications>
                </div>

                <button @click="ChatBoxOn" class="iconbutton">
                    <img class="w-6 h-6 theme-icon" src="/icons/message.svg" alt="">
                </button>

                <div id="chatbox" class="absolute w-56 rounded-b-lg theme-color top-14 left-[4.2%] flex-col hidden z-10">
                   <Chats></Chats>
                </div>
                
                <button @click="ExploreBoxOn" class="iconbutton">
                    <img class="w-6 h-6 theme-icon" src="/icons/apps.svg" alt="">
                </button>

                <div id="explore" class="absolute theme-color-light w-full h-full rounded-b-lg theme-color-white top-14 left-0 z-10 opacity-0 flex-col hidden">
                   <Exploreapps></Exploreapps>
                </div>
            </div>
        </div>
        <div class="nav-right flex items-center md:gap-8">
    <div class="relative">
    <div class="absolute left-4 top-3">
        <img class="h-5 w-5 theme-icon" src="/icons/search.svg" alt="">
    </div>
   <input class="w-full rounded-full  p-2  pl-10 focus:outline-none theme-color-light theme-color-text" type="text" placeholder="Arama">
</div>   
        <button @click="SettingsOn">
            <img class="w-12 rounded-full mr-4" src="/images/person.jpg" alt="">
        </button>
        <div id="pp-settings" class="absolute w-56 rounded-b-lg theme-color top-14 md:left-[88%] left-[40%] z-10 flex-col hidden">
                   <PpSettings></PpSettings>
        </div>
        </div>

        <Alert class="absolute top-[65%] left-[20%] md:top-[85%] md:left-[80%] z-20"></Alert>

    </div>
</template>

<style>
.iconbutton{
    display: flex;
    align-items: center;
    justify-content: center;   
    width: 2.5rem;
    height: 2.5rem;
    border-radius: 0.75rem;
}
.iconbutton:hover{
    background-color: #5F9DF7;
    transition: background-color 0.25s;
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
.theme-icon{
    filter: invert(0);
}
</style>

<script setup>

</script>