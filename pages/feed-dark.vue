<template>
    <div class="theme-color-light min-h-screen max-w-full">
        <LazyNavbarDark></LazyNavbarDark>
        <div class="content flex mt-4">
            <div class="con-left hidden basis-5/12 mr-4 md:flex justify-end">
                <LazyRecPagesDark></LazyRecPagesDark>
            </div>
            <div class="md:con-middle md:basis-5/12 md:mr-6 md:ml-6 flex items-center flex-col">
                <LazyPublishDark></LazyPublishDark>
                <LazyPostsDark></LazyPostsDark>
                <LazyPostsDark></LazyPostsDark>
            </div>
            <div class="con-right hidden md:basis-5/12 ml-4 md:flex justify-start">
                <LazyStories></LazyStories>
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
</style>