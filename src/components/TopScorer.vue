<template>
    <section id="home" class="min-h-[630px] pt-[92px] bg-gradient-to-b from-[#F9FAFC] to-white">
        <div class="w-full min-h-[630px] topScorer relative">
            <div>
                <img src="/img/bas-gray.png" alt=""
                    class="opacity-[12%] mix-blend-luminosity absolute z-[1] top-[20px] w-[556.5px] ball">
                <p
                    class="font-[Kanit-Bold] text-[80px] leading-[85%] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text w-[430px] uppercase absolute top-[15%] left-[8%] z-[2] top_text">
                    Top scorer to the final match</p>
                <img src="/img/player.png" class="absolute z-[3] left-[17%] top-[10%] w-[720px] top_player" alt="">


                <div class="w-[365px] absolute z-[4] left-[34%] top-[79%] flex flex-col gap-[24px] top_button">
                    <p class="font-[DMSans] text-[18px] top__text">
                        The EuroLeague Finals Top Scorer is the individual
                        award for the player that gained the highest points in
                        the EuroLeague Finals</p>
                    <button
                        class="uppercase px-[32px] py-[12px] bg-[#262626] rounded-[6px] opacity-100 text-white font-[DMSans-Bold] text-[20px] w-fit button_">Continue
                        reading</button>
                </div>

            </div>

            <div class="float-right translate-y-[20%] flex flex-col gap-[24px] today">
                <p
                    class="px-[16px] py-[4px] rounded-[3px] bg-[#E1E8F0] text-[#B8C2CE] font-[DMSans-Medium] text-[20px] w-fit">
                    Today</p>

                <div class="flex flex-col gap-[24px] today_block">
                    <div
                        class="bg-[url(/img/african-athlete.png)] h-[233px] w-[270px] bg-contain relative rounded-[6px] bg-no-repeat">
                        <div
                            class="absolute bottom-0 h-[132px] w-full bg-gradient-to-t from-[#F2F2F2] to-transparent rounded-[6px] flex items-end pb-[10px] pl-[16px]">
                            <div class="w-[200px] flex flex-col gap-[4px]">
                                <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">Race98 - 03 June 2023</p>
                                <p class="font-[Kanit-Regular] leading-[124%]">Ethiopian runners took the top four
                                    spots.
                                </p>
                            </div>
                        </div>
                    </div>

                    <div
                        class="bg-[url(/img/formula1.png)] h-[233px] w-[270px] bg-contain relative rounded-[6px] bg-no-repeat">
                        <div
                            class="absolute bottom-0 h-[132px] w-full bg-gradient-to-t from-[#F2F2F2] to-transparent rounded-[6px] flex items-end pb-[10px] pl-[16px]">
                            <div class="w-[200px] flex flex-col gap-[4px]">
                                <p class="font-[DMSans-Medium] text-[10px] text-[#262626]">INDYCAR - 03 June 2023</p>
                                <p class="font-[Kanit-Regular] leading-[124%]">IndyCar Detroit: Dixon quickest in second
                                    practice</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>


    </section>
</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .topScorer {
        width: 1440px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1500px) {
    .topScorer {
        width: 1240px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1300px) {
    .topScorer {
        width: 1000px;
        margin: 0 auto;
        height: 1000px;
        display: flex;
    }

    .today {
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
    }

    .today_block {
        flex-direction: row;
    }

    .top_text {
        top: 110px;
    }

    .top_player {
        top: 90px;
        left: 180px;
    }

    .top_button {
        top: 560px;
        left: 420px;
    }

}

@media screen and (max-width: 1050px) {
    .topScorer {
        width: 880px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 920px) {
    .topScorer {
        width: 768px;
        height: 900px;
        margin: 0 auto;
    }

    .ball {
        width: 500px;
    }

    .top_text {
        width: 390px;
        font-size: 70px;
        left: 90px;
    }

    .top_player {
        width: 550px;
        top: 90px;
        left: 220px;
    }

    .top_button {
        top: 460px;
        left: 370px;
    }
}

@media screen and (max-width: 800px) {
    .topScorer {
        width: auto;
        height: 800px;
        margin: 0 20px;
    }

    .ball {
        width: 400px;
    }

    .top_text {
        width: 330px;
        font-size: 60px;
        left: 80px;
        top: 80px;
    }

    .top_player {
        width: 480px;
        top: 70px;
        left: 180px;
    }

    .top_button {
        width: 460px;
        top: 380px;
        left: 300px;
    }

    .top__text {
        font-size: 16px;
    }

    .button_ {
        padding: 10px 24px;
        font-size: 18px;
    }
}

@media screen and (max-width: 800px) {
    .topScorer {
        height: 730px;
    }

    .ball {
        width: 350px;
    }

    .top_text {
        width: 240px;
        font-size: 45px;
        left: 70px;
        top: 80px;
    }

    .top_player {
        width: 380px;
        top: 70px;
        left: 140px;
    }

    .top_button {
        width: 280px;
        top: 310px;
        left: 240px;
    }

    .top__text {
        font-size: 16px;
    }

    .button_ {
        padding: 10px 16px;
        font-size: 18px;
    }
}

@media screen and (max-width: 600px) {
    .topScorer {
        height: 950px;
    }

    .today {
        width: 100%;
    }

    .today_block {
        justify-content: center;
        margin: 0 auto;
        flex-direction: column;
    }
}

@media screen and (max-width: 550px) {
    .topScorer {
        height: 900px;
    }

    .ball {
        width: 270px;
    }

    .top_text {
        width: 200px;
        font-size: 35px;
        left: 50px;
        top: 70px;
    }

    .top_player {
        width: 300px;
        top: 50px;
        left: 100px;
    }

    .top_button {
        width: 200px;
        top: 250px;
        left: 200px;
    }

    .top__text {
        font-size: 14px;
    }

    .button_ {
        padding: 8px 10px;
        font-size: 14px;
    }
}

@media screen and (max-width: 430px) {
    .topScorer {
        height: 820px;
    }

    .ball {
        width: 250px;
    }

    .top_text {
        width: 160px;
        font-size: 28px;
        left: 40px;
        top: 70px;
    }

    .top_player {
        width: 250px;
        top: 30px;
        left: 90px;
    }

    .top_button {
        width: 210px;
        top: 200px;
        left: 130px;
    }

    .top__text {
        font-size: 13px;
    }

    .button_ {
        padding: 8px 10px;
        font-size: 13px;
    }
}
</style>