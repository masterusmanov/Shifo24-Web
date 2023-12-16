<template>
    <div @click="open" class="w-full h-[180vh] bg-black bg-opacity-20 top-0 right-0 left-0 flex justify-center items-center fixed z-50 border-none outline-none">
        <div class="w-full bg-white self-start max-w-screen-md max-h-screen-xl border border-black">
            <div class="flex items-center h-[60px] px-[10px] mt-[3px]">
                <div class="w-[85%] flex items-center gap-2 md:w-[40%]">
                    <svg xmlns="http://www.w3.org/2000/svg" width="31" height="29" viewBox="0 0 31 29" fill="none">
                        <path d="M21.9011 0.517334C26.4897 0.517334 30.2084 4.29643 30.2084 9.58717C30.2084 20.1687 18.8802 26.2152 15.1042 28.4827C12.1166 26.6884 4.40438 22.5314 1.31104 15.6337H8.40699L9.81772 13.2816L14.349 20.8398L17.4695 15.6337H22.6563V12.6105H15.7597L14.349 14.9626L9.81772 7.40437L6.6972 12.6105H0.317188C0.111771 11.6475 0 10.6393 0 9.58717C0 4.29643 3.77605 0.517334 8.3073 0.517334C11.1167 0.517334 13.5938 2.02897 15.1042 3.54061C16.6146 2.02897 19.0917 0.517334 21.9011 0.517334Z" fill="#067A9E"/>
                    </svg>
                    <h1 class="font-[500] text-[26.5px] font-rubik">Shifo24</h1>
                </div>
                <div @click="emitClose" class="ml-[25px]">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20" fill="none">
                        <path d="M19.7076 18.2925C19.8005 18.3854 19.8742 18.4957 19.9245 18.6171C19.9747 18.7385 20.0006 18.8686 20.0006 19C20.0006 19.1314 19.9747 19.2615 19.9245 19.3829C19.8742 19.5043 19.8005 19.6146 19.7076 19.7075C19.6147 19.8004 19.5044 19.8741 19.383 19.9244C19.2616 19.9747 19.1315 20.0006 19.0001 20.0006C18.8687 20.0006 18.7386 19.9747 18.6172 19.9244C18.4958 19.8741 18.3855 19.8004 18.2926 19.7075L10.0001 11.4138L1.70757 19.7075C1.51993 19.8951 1.26543 20.0006 1.00007 20.0006C0.734704 20.0006 0.480208 19.8951 0.292568 19.7075C0.104927 19.5199 -0.000488276 19.2654 -0.000488281 19C-0.000488286 18.7346 0.104927 18.4801 0.292568 18.2925L8.58632 10L0.292568 1.70751C0.104927 1.51987 -0.000488281 1.26537 -0.000488281 1.00001C-0.000488281 0.734643 0.104927 0.480147 0.292568 0.292507C0.480208 0.104866 0.734704 -0.000549316 1.00007 -0.000549316C1.26543 -0.000549316 1.51993 0.104866 1.70757 0.292507L10.0001 8.58626L18.2926 0.292507C18.4802 0.104866 18.7347 -0.000549322 19.0001 -0.000549316C19.2654 -0.000549311 19.5199 0.104866 19.7076 0.292507C19.8952 0.480147 20.0006 0.734643 20.0006 1.00001C20.0006 1.26537 19.8952 1.51987 19.7076 1.70751L11.4138 10L19.7076 18.2925Z" fill="#424259"/>
                      </svg>
                </div>
            </div>
            <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownHoverButton">
                <li>
                    <a href="#about" @click="emitClose" class="text-[18px] block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Biz haqimizda</a>
                </li>
                <li>
                    <a href="#feature" @click="emitClose" class="text-[18px] block my-[22px] px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Hususiyatlar</a>
                </li>
                <li>
                    <a href="#patient" @click="emitClose" class="text-[18px] block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white font-rubik">Bemorlar</a>
                </li>
                <li class="my-[32px] ">
                    <button class="w-[92%] mx-4 font-[500] py-[10px] px-[20px] border border-[#2588AF] rounded-lg font-rubik text-[#2588AF] hover:text-white hover:bg-[#2588AF]">Bog'lanish</button>
                </li>
            </ul>
        </div>
    </div>
</template>

<script setup>
import { defineEmits } from 'vue';

const emit = defineEmits(['close']);

function emitClose() {
  emit('close');
}
</script>

<style lang="scss" scoped>
</style>