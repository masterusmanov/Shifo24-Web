<template>
   <header class="bg-[#FFF] sticky top-0 z-50">
        <div class="container mx-auto h-[70px] flex justify-center items-center md:px-4 lg:px-0 xl:px-4 2xl:px-0">
            <div class="w-[85%] flex items-center gap-2 md:w-[40%]">
                <svg xmlns="http://www.w3.org/2000/svg" width="31" height="29" viewBox="0 0 31 29" fill="none">
                    <path d="M21.9011 0.517334C26.4897 0.517334 30.2084 4.29643 30.2084 9.58717C30.2084 20.1687 18.8802 26.2152 15.1042 28.4827C12.1166 26.6884 4.40438 22.5314 1.31104 15.6337H8.40699L9.81772 13.2816L14.349 20.8398L17.4695 15.6337H22.6563V12.6105H15.7597L14.349 14.9626L9.81772 7.40437L6.6972 12.6105H0.317188C0.111771 11.6475 0 10.6393 0 9.58717C0 4.29643 3.77605 0.517334 8.3073 0.517334C11.1167 0.517334 13.5938 2.02897 15.1042 3.54061C16.6146 2.02897 19.0917 0.517334 21.9011 0.517334Z" fill="#067A9E"/>
                </svg>
                <h1 class="font-bold text-[26.5px] font-rubik">Shifo24</h1>
            </div>
            <div id="navbar" class="hidden md:flex w-[70%] justify-end items-center gap-6 lg:gap-14 font-bold font-rubik">
                <router-link to="#">Biz haqimizda</router-link>
                <router-link to="#">Hususiyatlar</router-link>
                <router-link to="#">Bemorlar</router-link>
                <button class="font-[600] py-2 px-3 border border-[#2588AF] rounded-lg font-rubik">Bog'lanish</button>
            </div>
            <div id="menu" class="w-[10%] float-right md:hidden">            
                <button id="dropdownHoverButton" data-dropdown-toggle="dropdownHover" data-dropdown-trigger="hover" class="" type="button float-right"><i class='bx bx-menu text-[36px]'></i></button>
                    <!-- Dropdown menu -->
                    <div id="dropdownHover" class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-[120px] dark:bg-gray-700">
                        <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownHoverButton">
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Biz haqimizda</a>
                            </li>
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Hususiyatlar</a>
                            </li>
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Bemorlar</a>
                            </li>
                        </ul>
                    </div>
            </div>
        </div>
   </header>
</template>

<script setup>
    import { Dropdown } from 'flowbite';
</script>

<style lang="scss" scoped>
   
</style>