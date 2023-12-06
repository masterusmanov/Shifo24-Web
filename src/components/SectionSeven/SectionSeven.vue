<template>
    <section class="px-2 mt-[104px] md:mt-[128px] xl:mt-[200px]">
        <div class="container mx-auto ">
            <h1 class="text-[27px] text-[#424259] font-[700] xl:text-[36px] pt-[48px]">Bizning mijozlarimiz fikrlari</h1>
            <p class="text-[16px] text-[#424259] font-[400] mt-[16px]">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
        </div>
        <Card class=" md:hidden mt-[40px]"/>
        <CardTwo class="hidden md:block mt-[72px] xl:mt-[88px]"/>
        <div class="container mx-auto md:mt-[97px]">
            <p class="text-[16px] font-[500] text-[#42425]">Xizmatlarimiz <span class="text-[16px] font-[500] text-[#2588AF]">100+</span> odamlarni xursand qilgan</p>
        </div>
    </section>
</template>

<script setup>
    import Card from '../Card.vue';
    import CardTwo from '../CardTwo.vue';
</script>

<style lang="scss" scoped>

</style>