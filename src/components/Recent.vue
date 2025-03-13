<template>
    <div class="flex gap-[24px] recent">
        <!-- Recent News -->
        <div class="flex flex-col gap-[24px]">
            <p class="font-[Kanit-Medium] text-[28px]">Recent News</p>

            <div class="flex gap-[36px] baku">
                <div
                    class="bg-[url(/img/karate.png)] h-[300px] w-[270px] bg-contain relative rounded-[6px] bg-no-repeat">
                    <div
                        class="absolute bottom-0 h-[82px] w-full bg-[linear-gradient(73deg,_rgba(179,149,119)_0%,_rgba(229,201,159)_100%)] rounded-b-[6px] flex items-end pb-[10px] pl-[16px]">
                        <div class="w-[200px] flex flex-col gap-[4px]">
                            <p class="font-[DMSans-Medium] text-[10px] text-[#EBEEF3]">Day 5 Highlights</p>
                            <p class="font-[Kanit-Regular] leading-[124%] text-[#EBEEF3]">Baku 2023 World Taekwondo
                                Championships
                            </p>
                        </div>
                    </div>
                </div>

                <!-- More info -->

                <div class=" bg-[#EBEEF3] w-[270px] h-[300px] rounded-[6px] p-[16px]">
                    <div class="flex flex-col h-full justify-between items-center">
                        <div class="flex items-center gap-[8px]">
                            <img src="/img/taekwondo.png" alt="" class="w-[70px]">
                            <div class="flex flex-col gap-[4px]">
                                <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">#Pollar. 87 - 12 July 2023
                                </p>
                                <p class="font-[Kanit-Regular] text-[16px] text-[#262626] leading-[120%]">Baku 2023
                                    Taekwondo Championships</p>
                            </div>
                        </div>

                        <div class="flex items-center gap-[8px]">
                            <img src="/img/golf.png" alt="" class="w-[70px]">
                            <div class="flex flex-col gap-[4px]">
                                <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">#Pollar. 87 - 12 July 2023
                                </p>
                                <p class="font-[Kanit-Regular] text-[16px] text-[#262626] leading-[120%]">Baku 2023
                                    Taekwondo Championships</p>
                            </div>
                        </div>

                        <div class="flex items-center gap-[8px]">
                            <img src="/img/cricket.png" alt="" class="w-[70px]">
                            <div class="flex flex-col gap-[4px]">
                                <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">#Pollar. 87 - 12 July 2023
                                </p>
                                <p class="font-[Kanit-Regular] text-[16px] text-[#262626] leading-[120%]">Baku 2023
                                    Taekwondo Championships</p>
                            </div>
                        </div>

                        <button
                            class="flex justify-center items-center bg-[#B8C2CE] rounded-[6px] w-[80px] h-[28px] gap-[8px] cursor-pointer">
                            <p class="font-[DMSans-Medium] text-white text-[14px]">More</p>
                            <img src="/ui/arrow_small.png" alt="" class="w-[10px]">
                        </button>
                    </div>

                </div>
            </div>
        </div>

        <!-- Clubs Ranking -->

        <div class="flex flex-col gap-[24px] flex-1">
            <p class="font-[Kanit-Medium] text-[28px]">Clubs Ranking</p>

            <div class="py-[12px] bg-gray-100 font-[DMSans] rounded-[6px] h-full">
                <table class="w-full text-left border-collapse">
                    <thead>
                        <tr class="text-gray-700 text-sm font-semibold _table_">
                            <th class="pl-[16px] pb-[8px]">Club</th>
                            <th class="px-[4px]">GP</th>
                            <th class="px-[4px]">W</th>
                            <th class="px-[4px]">D</th>
                            <th class="px-[4px]">L</th>
                            <th class="px-[4px]">F</th>
                            <th class="px-[4px]">A</th>
                            <th class="px-[4px]">GD</th>
                        </tr>
                    </thead>
                    <tbody >
                        <tr v-for="(team, index) in teams" :key="index" class="border-t first:border-none table_">
                            <td class=" flex items-center gap-2 ml-[16px] my-[8px]">
                                <span class="font-semibold text-gray-700 w-6">{{ index + 1 }}</span>
                                <img :src="team.logo" alt="Club Logo" class="w-6 h-6" />
                                <span class="text-gray-900">{{ team.name }}</span>
                            </td>
                            <td class="px-[4px]">{{ team.gp }}</td>
                            <td class="px-[4px]">{{ team.w }}</td>
                            <td class="px-[4px]">{{ team.d }}</td>
                            <td class="px-[4px]">{{ team.l }}</td>
                            <td class="px-[4px]">{{ team.f }}</td>
                            <td class="px-[4px]">{{ team.a }}</td>
                            <td class="font-bold px-[4px]">{{ team.gd }}</td>
                        </tr>
                    </tbody>
                </table>
            </div>

        </div>
    </div>

</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .recent {
        width: 1440px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1500px) {
    .recent {
        width: 1240px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1300px) {
    .recent {
        width: 1000px;
        margin: 80px auto;
        flex-direction: column;
    }
}

@media screen and (max-width: 1050px) {
    .recent {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .recent {
        width: 768px;
    }
}

@media screen and (max-width: 920px) {
    .recent {
        width: auto;
        margin: 80px 20px;
    }
}

@media screen and (max-width: 600px) {
    .baku{
        flex-direction: column;
        justify-content: center;
        margin: 0 auto;
    }
}

@media screen and (max-width: 470px) {
    .table_ td:nth-child(1) span{
        font-size: 14px;
    }

    .table_ td:nth-child(1) img{
        width: 16px;
        height: 16px;
    }

    .table_ td:nth-child(2),
    .table_ td:nth-child(3),
    .table_ td:nth-child(4),
    .table_ td:nth-child(5),
    .table_ td:nth-child(6),
    .table_ td:nth-child(7),
    .table_ td:nth-child(8){
        font-size: 12px;
    }

    ._table_ th{
        font-size: 12px;
    }
}
</style>

<script setup>
import { ref } from "vue";

const teams = ref([
    {
        name: "Manchester City",
        logo: "/img/mancity.png",
        gp: 38,
        w: 29,
        d: 6,
        l: 3,
        f: 99,
        a: 26,
        gd: 73,
    },
    {
        name: "Liverpool",
        logo: "/img/liverpool.png",
        gp: 38,
        w: 28,
        d: 8,
        l: 2,
        f: 94,
        a: 26,
        gd: 68,
    },
    {
        name: "Chelsea",
        logo: "/img/chelsea.png",
        gp: 38,
        w: 21,
        d: 11,
        l: 6,
        f: 76,
        a: 33,
        gd: 43,
    },
    {
        name: "Tottenham Hotspur",
        logo: "/img/tottenham.png",
        gp: 38,
        w: 22,
        d: 5,
        l: 11,
        f: 69,
        a: 40,
        gd: 29,
    },
    {
        name: "Arsenal",
        logo: "/img/arsenal.png",
        gp: 38,
        w: 22,
        d: 3,
        l: 13,
        f: 61,
        a: 48,
        gd: 13,
    },
    {
        name: "Manchester United",
        logo: "/img/manuni.png",
        gp: 38,
        w: 16,
        d: 10,
        l: 12,
        f: 57,
        a: 57,
        gd: 0,
    },
]);
</script>