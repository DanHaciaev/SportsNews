<template>
    <div class="bg-[#EBEEF3] mx-[135px] my-[80px] rounded-[6px] flex flex-col football">
        <div class="relative bg-[url(/img/lionel-messi.png)] rounded-t-[6px] w-full h-[503px] bg-cover bg-no-repeat">
            <div class="absolute inset-0 bg-black/60 h-[503px] rounded-t-[6px]"></div>

            <div class="relative z-10 p-[32px] flex flex-col justify-between h-full">
                <p
                    class="text-white border-[2px] border-[#EBEEF3] px-[20px] py-[4px] w-fit rounded-[3px] font-[DMSans-Medium] text-[20px]">
                    Football
                </p>

                <div class="flex flex-col gap-[8px]">
                    <p class="font-[DMSans] text-[18px] text-white">Agence France-Presse - 04 June 2023</p>
                    <p class="font-[Kanit-Bold] text-[36px] text-white leading-[100%]">Lionel Messi Leaving Ligue 1 Team
                        Paris Saint-Germain, Club Confirms
                    </p>
                    <p class="font-[DMSans-Medium] text-[20px] text-white">The EuroLeague Finals Top Scorer is the
                        individual award for the player that gained the highest points in the EuroLeague Finals</p>
                </div>
            </div>
        </div>

        <div class="flex w-[470px] items-center justify-between mb-[24px] mt-[24px] mr-[16px] ml-auto arrow">
            <button
                class="w-[70px] h-[46px] rounded-[3px] bg-[#BAB8B8] flex justify-center items-center cursor-pointer">
                <img src="/ui/arrow_left.png" alt="" class="w-[24px]">
            </button>
            <div class="bg-[#262626] w-[35px] rounded-[50%] flex justify-center items-center">
                <p class="font-[Kanit-Medium] text-[24px] text-[#EBEEF3]">1</p>
            </div>
            <p class="font-[Kanit-Light] text-[24px] text-[#262626] opacity-[60%]">2</p>
            <p class="font-[Kanit-Light] text-[24px] text-[#262626] opacity-[60%]">3</p>
            <p class="font-[Kanit-Light] text-[24px] text-[#262626] opacity-[60%]">4</p>
            <button
                class="w-[70px] h-[46px] rounded-[3px] bg-[#262626] flex justify-center items-center cursor-pointer">
                <img src="/ui/arrow_right.png" alt="" class="w-[24px]">
            </button>
        </div>
    </div>
</template>


<style scoped>
@media screen and (max-width: 1920px) {
    .football {
        width: 1440px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1500px) {
    .football {
        width: 1240px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1300px) {
    .football {
        width: 1000px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1050px) {
    .football {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .football {
        width: 768px;
    }
}

@media screen and (max-width: 800px) {
    .football {
        width: auto;
        margin: 80px 20px;
    }
}

@media screen and (max-width: 600px) {
    .arrow{
        width: auto;
        gap: 24px;
    }

    .arrow button{
        width: 50px;
        height: 30px;
    }

    .arrow div:nth-child(1){
        width: 25px;
    }
}
</style>