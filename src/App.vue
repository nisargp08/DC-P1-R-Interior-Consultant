<template>
<div id="app">
    <div class="flex flex-col bg-primary min-h-screen p-3 text-white">
        <header>
            <div class="flex items-center justify-between">
                <div class="border border-white p-2">
                    <p class="font-crimsonPro text-sm uppercase font-thin leading-4">this interior</p>
                </div>
                <div>
                    <svg class="h-8 w-8 fill-current" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                    </svg>
                </div>
            </div>
        </header>
        <main class="flex-1">
            <div class="mt-10">
                <h1 class="font-lora font-normal text-4xl leading-12">Modern interior</h1>
            </div>
            <div class="w-64 mt-6">
                <h2 class="font-montserrat font-light text-sm leading-4">A full-Service residential & commercial interior design and staging company
                    offering professional organizing & eco-services.</h2>
            </div>
            <div class="mt-6">
                <div class="flex items-center">
                    <p class="font-montserrat font-semibold text-sm leading-4">Read more</p>
                    <div class="ml-4">
                        <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
                        </svg>
                    </div>
                </div>
            </div>
            <div class="mt-6">
                <div>
                    <img class="rounded-lg" src="@/assets/images/photo1.png" alt="Designed Home">
                </div>
                <div class="relative pl-12 pr-4 -mt-12">
                    <div class="flex flex-col rounded-lg bg-primary p-2 shadow-3xl">
                        <div class="flex">
                            <div class="flex items-center justify-center w-12 h-12">
                                <img class="w-8 rounded-full" src="@/assets/images/photo2.png" alt="Interior Designer">
                            </div>
                            <div class="flex flex-col justify-center ml-2">
                                <p class="font-montserrat font-medium text-xs leading-4">Aliza Webber</p>
                                <p class="font-montserrat font-medium text-xxs text-secondary">Interior designer</p>
                            </div>
                        </div>
                        <div class="mt-2 pl-2 w-48">
                            <h3 class="font-lora font-bold text-lg leading-6">Designed in 2020 by Aliza Webber</h3>
                        </div>
                    </div>
                </div>
            </div>
        </main>
        <footer>
            <div class="flex items-center justify-center">
              <div class="border-t border-tertiary">
                <p class="font-montserrat text-tertiary pt-3 pb-6 font-semibold leading-4 text-sm">Nisarg Patel @ DevChallenges.io</p>
              </div>
            </div>
        </footer>
    </div>
</div>
</template>

<script>
export default {
    name: 'App',
    components: {}
}
</script>

<style lang="scss">
#app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
</style>
