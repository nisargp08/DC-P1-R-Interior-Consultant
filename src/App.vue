<template>
<div id="app">
    <div class="bg-primary text-white">
        <div class="flex flex-col p-3 lg:p-10 min-h-screen lg:max-w-screen-lg lg:mx-auto xl:max-w-screen-xl xl:py-10 xl:px-0">
          <header>
              <div class="flex items-center justify-between">
                  <div class="border border-white p-2">
                      <p class="font-crimsonPro text-sm uppercase font-thin leading-4">this interior</p>
                  </div>
                  <div class="lg:hidden">
                    <button @click="toggle" class="trasition duration-300 ease-in-out  hover:text-red-600 focus:outline-none">
                      <svg class="h-8 w-8 fill-current" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                      </svg>
                    </button>
                  </div>
                  <div :class="{ 'hidden' : !isOpen, 'block' : isOpen}" class="fixed inset-0 z-10 bg-primary text-white lg:flex lg:static lg:w-5/12">
                    <div class="flex flex-col h-full lg:flex-1">
                      <div class="self-end lg:hidden">
                        <button @click="toggle" class="p-2 trasition duration-300 ease-in-out hover:text-red-600 focus:outline-none">
                          <svg class="w-8 h-8 fill-current" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
                          </svg>
                        </button>
                      </div>
                      <nav class="flex items-center justify-center flex-1 text-center">
                          <div class="lg:flex lg:w-full lg:justify-between">
                            <div class="font-montserrat font-bold text-lg leading-6 cursor-pointer"><p>Home</p></div>
                            <div class="font-montserrat mt-8 text-lg leading-6 font-medium cursor-pointer trasition duration-300 ease-in-out hover:text-red-600 lg:mt-0"><p>Collection</p></div>
                            <div class="font-montserrat mt-8 text-lg leading-6 font-medium cursor-pointer trasition duration-300 ease-in-out hover:text-red-600 lg:mt-0"><p>About</p></div>
                            <div class="font-montserrat mt-8 text-lg leading-6 font-medium cursor-pointer trasition duration-300 ease-in-out hover:text-red-600 lg:mt-0"><p>Contact</p></div>
                          </div>
                      </nav>
                    </div>
                  </div>
              </div>
          </header>
          <main class="flex-1 lg:mt-32 lg:flex">
              <div class="lg:w-1/3 xl:w-1/3">
                <div class="mt-10 lg:mt-6">
                    <h1 class="font-lora font-normal text-4xl leading-12 md:text-center lg:text-left">Modern interior</h1>
                </div>
                <div class="w-64 mt-6 md:w-full md:text-center lg:text-left xl:w-3/5">
                    <h2 class="font-montserrat font-light text-sm leading-4">A full-Service residential & commercial interior design and staging company
                        offering professional organizing & <br class="hidden xl:block"> eco-services.</h2>
                </div>
                <div class="mt-6">
                    <div class="flex items-center md:justify-center lg:justify-start">
                        <p class="font-montserrat font-semibold text-sm leading-4">Read more</p>
                        <div class="ml-4">
                            <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
                            </svg>
                        </div>
                    </div>
                </div>
              </div>
              <div class="mt-6 md:max-w-md md:mx-auto lg:max-w-1/2 xl:max-w-2xl xl:mr-0">
                  <div>
                      <img class="rounded-lg" src="@/assets/images/photo1.png" alt="Designed Home">
                  </div>
                  <div class="pl-12 pr-4 -mt-12 xl:flex xl:justify-end xl:-mt-16">
                      <div class="relative flex flex-col rounded-lg bg-primary p-2 shadow-3xl xl:w-1/2">
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
          <footer class="lg:mt-32">
              <div class="flex items-center justify-center">
                <div class="border-t border-tertiary">
                  <p class="font-montserrat text-tertiary pt-3 pb-6 font-semibold leading-4 text-sm">Nisarg Patel @ DevChallenges.io</p>
                </div>
              </div>
          </footer>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'App',
    data(){
      return {
        //Navigation bar open/close tracker
        isOpen : false,
      }
    },
    methods : {
      toggle(){
        //Toggle display state
        this.isOpen = !this.isOpen;
      }
    },
    components: {},
}
</script>

<style lang="scss">
#app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
</style>
