<template>
    <div class="flex flex-col gap-[24px] article">
        <p class="font-[Kanit-Medium] text-[28px]">Sports Article</p>

        <div class="flex w-full justify-between articles">
            <div class="w-[370px] h-[500px] flex flex-col gap-[24px]" v-for="(article, index) in articles" :key="index">
                <div class="bg-cover relative w-full h-[280px] p-[16px] rounded-[6px]"
                    :style="`background-image: url(${article.photo})`">
                    <p
                        class="text-white font-[DMSans] text-[12px] absolute right-[16px] rounded-[4px] border-[1px] px-[10px] py-[6px]">
                        {{ article.sport }}</p>
                </div>
                <div class="flex flex-col gap-[16px]">
                    <div class="flex items-center gap-[8px]">
                        <img :src="article.photo_user" alt="" class="w-[44px] h-[44px]">
                        <p class="font-[Roboto-Medium] text-[14px]">{{ article.name_user }}</p>
                    </div>

                    <p class="font-[DMSans-Medium] text-[14px] text-[#262626] opacity-[60%]">{{ article.date }}</p>

                    <p class="font-[Kanit-Regular] text-[22px] text-[#262626]">{{ article.text }}</p>

                    <p class="font-[DMSans-Medium] text-[16px] text-[#262626] opacity-[60%]">{{ article.another }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .article {
        width: 1440px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1500px) {
    .article {
        width: 1240px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1300px) {
    .article {
        width: 1000px;
        margin: 80px auto;
    }

    .articles{
        flex-wrap: wrap;
        gap: 30px;
    }
}

@media screen and (max-width: 1050px) {
    .article {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .article {
        width: 768px;
    }

    .articles{
        justify-content: center;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1500px) {
    .article {
        width: auto;
        margin: 80px 20px;
    }
}
</style>

<script setup>
import { ref } from 'vue';

const articles = ref([
    {
        photo: '/img/basketball-equipment.png',
        photo_user: '/img/jakewill.png',
        sport: 'Basketball',
        name_user: 'Jake Will',
        date: '04 June 2023',
        text: '5 Exercises Basketball Players Should Be Using To Develop Strength',
        another: 'This article was written by Jake Willhoite from Healthlisted.com Strength in basketball isn’t all about a massive body mass or ripped muscles.'
    },
    {
        photo: '/img/hockey-players.png',
        photo_user: '/img/foxizacon.png',
        sport: 'Hockey',
        name_user: 'Foxi.zacon',
        date: '03 June 2023',
        text: 'Golden Knights out to fulfill owner’s quest to win Stanley Cup in 6th year',
        another: 'The Vegas Golden Knights will play the Florida Panthers in the Stanley Cup Final beginning Saturday.'
    },
    {
        photo: '/img/badminton-racquet.png',
        photo_user: '/img/bonglozada.png',
        sport: 'Badminton',
        name_user: 'Bong Lozada',
        date: '01 June 2023',
        text: '‘Outdoor’ Badminton Gets Support From Local Federation',
        another: 'The Badminton World Federation is developing Air Badminton and the country’s governing body, Philippine Badminton Association.'
    }
])

</script>