<template>
    <section id="trending" class="bg-[#EBEEF3] rounded-[6px] h-[609px] mx-[135px] my-[30px] flex justify-between trending">
        <div class="my-[24px] mx-[24px] flex flex-col gap-[24px]">
            <p class="font-[Kanit-Medium] text-[28px]">Trending News</p>
            <div class="flex flex-col gap-[24px] news">
                <div class="flex gap-[24px] w-[515px] items-center art">
                    <img src="/img/horse.png" alt="" class="w-[234px] art_img">

                    <div class="flex flex-col gap-[4px]">
                        <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">Race98 - 03 June 2023</p>
                        <p class="font-[Kanit-Medium] text-[18px] text-[#262626]">6-Year-Old Horse Dies at Belmont Park
                            After Race Injury</p>
                        <p class="font-[DMSans] text-[12px] text-[#262626]">NEW YORK—A 6-year-old horse died after being
                            injured in a race at Belmont Park ahead of next
                            week’s
                        </p>
                    </div>
                </div>

                <div class="flex gap-[24px] w-[515px] art">
                    <img src="/img/cycling.png" alt="" class="w-[234px] art_img">

                    <div class="flex flex-col gap-[4px] pt-[12px] border-t-[1px] border-[#B8C2CE]">
                        <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">Jony.Ls - 03 June 2023</p>
                        <p class="font-[Kanit-Medium] text-[18px] text-[#262626]">Savilia Blunk Embraces Longer Season
                            with
                            World Cup</p>
                        <p class="font-[DMSans] text-[12px] text-[#262626]">Last year, Savilia Blunk took a more
                            conservative approach to her first season as an Elite Class athlete, skipping some
                        </p>
                    </div>
                </div>

                <div class="flex gap-[24px] w-[515px] art">
                    <img src="/img/box.png" alt="" class="w-[234px] art_img">

                    <div class="flex flex-col gap-[4px] pt-[12px] border-t-[1px] border-[#B8C2CE]">
                        <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">King.F - 03 June 2023</p>
                        <p class="font-[Kanit-Medium] text-[18px] text-[#262626]">Ryan Garcia is fighting again, this
                            time
                            on social media</p>
                        <p class="font-[DMSans] text-[12px] text-[#262626]">Boxing star Ryan Garcia and his promoter,
                            Hall
                            of Fame fighter Oscar De La Hoya, reignited their war of words via Twitter on
                        </p>
                    </div>
                </div>
            </div>

        </div>


        <div
            class="relative h-full w-full bg-[url('/img/sportsman-drinking.png')] bg-cover bg-no-repeat bg-center rounded-[6px] cycling">
            <div class="absolute inset-0 bg-black/60 rounded-[6px]"></div>

            <div class="relative z-10 p-[32px] flex flex-col justify-between h-full">
                <p
                    class="text-white border-[2px] border-[#EBEEF3] px-[20px] py-[4px] w-fit rounded-[3px] font-[DMSans-Medium] text-[20px]">
                    Cycling
                </p>

                <div class="flex flex-col gap-[8px]">
                    <p class="font-[DMSans] text-[18px] text-white">Debits - 03 June 2023</p>
                    <p class="font-[Kanit-Bold] text-[36px] text-white leading-[100%]">
                        DISCOVER THE MEMBER BENEFITS OF USA CYCLING!
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .trending {
        width: 1440px;
        margin: 30px auto;
    }
}

@media screen and (max-width: 1500px) {
    .trending {
        width: 1240px;
    }
}

@media screen and (max-width: 1300px) {
    .trending {
        width: 1000px;
        height: fit-content;
        flex-direction: column;
    }

    .news {
        display: flex;
        justify-content: center;
        margin: 0 auto;
    }

    .cycling {
        display: flex;
        justify-content: center;
        margin: 0 auto 24px;
        width: 600px;
        height: 600px;
    }
}

@media screen and (max-width: 1050px) {
    .trending {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .trending {
        width: 768px;
    }
}

@media screen and (max-width: 920px) {
    .trending {
        width: auto;
        margin: 30px 20px;
    }
}

@media screen and (max-width: 670px) {
    .news{
        margin: 0 auto;
        justify-content: center;
    }

    .cycling{
        width: auto;
        margin: 0 20px 24px;
    }
}

@media screen and (max-width: 600px) {
    .news{
        margin: 0 auto;
        gap: 40px;
    }

    .art{
        width: 100%;
        flex-direction: column;
        align-items: center;
    }

    .art:nth-child(1) div:nth-child(2){
        border-top: 1px solid #B8C2CE;
        padding-top: 12px;
    }

}
</style>