<template>
    <div class="flex flex-col md:flex-row ">
        <div class="flex flex-col left md:basis-1/2 md:h-screen h-[65vh] bg-[#082032] ">
            <span class="index-text-style ml-[5%] mt-[5%]">Gen Z <br> NB, SİZİN İÇİN BİR SOSYAL MEDYA!</span>
            
                <div class="flex flex-col self-center md:w-[70%]">
            <NuxtLink to="feed-dark">
                <img class="w-full border-4 border-white" src="/images/dark-feed.png" alt="">
                <p class="text-white ml-[25%] text-xl font-bold">Feed Sayfası Örneği (Tıkla)</p>
            </NuxtLink>
            </div>
            
            
            
            
        </div>
        <div class="flex right md:basis-1/2 md:h-screen h-[65vh] bg-[#334756] items-center">

            
                <div class="mx-auto w-full max-w-xs">
<div class="relative mb-3">
    <label class="absolute bg-white px-1 text-xs block text-gray-600 top-2 left-2">E-Posta</label>
    <div class="mt-1">
        <input type="text" value="e-posta@ornekmail.com" class="border border-gray-300 focus:outline-blue-400 rounded w-full h-14 p-3 pt-8 text-sm">
    </div>
</div>
<div class="relative mb-3">
    <label class="absolute bg-white px-1 text-xs block text-gray-600 top-2 left-2">Şifre</label>
    <div class="mt-1">
        <input type="password" value="xyz123" class="border border-gray-300 focus:outline-blue-400 rounded w-full h-14 p-3 pt-8 text-sm">
    </div>
    <button class="mt-4 rounded bg-blue-500 hover:bg-blue-600 text-white border-blue-700 w-32 h-10">Giriş Yap</button>

</div>
<a href="">şifremi unuttum</a>
<br>
<a href="">üye değil misin ? kayıt ol</a>
</div>

            </div>

            <Alert class="absolute md:top-[85%] md:left-[80%] top-[52%] left-[12%]"></Alert>
    </div>
</template>

<style>

.index-text-style {
  grid-area: text;
  font-family: 'Sarpanch', sans-serif;
  font-size: 10vmin;
  color: #1d9099;
  text-shadow: 0.5vmin 0.5vmin 0 #E79C10, -.5vmin -.5vmin 0 #D53A33;
}
</style>