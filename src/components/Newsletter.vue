<template>
    <div class="bg-[#EBEEF3] rounded-[6px] h-[385px] flex news">
        <div class="mt-[90px] ml-[66px] flex flex-col gap-[36px] news_input">
            <p
                class="font-[Kanit-Bold] text-[60px] leading-[85%] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text w-[510px] uppercase sub">
                Newsletter Subscription
            </p>

            <div class="flex h-[58px] w-[514px] input">
                <input type="text" placeholder="shovon.khan0099@gmail.com"
                    class="border w-full px-[16px] rounded-l-[6px]">
                <div class="flex justify-center items-center bg-[#262626] rounded-r-[6px] w-[74px]">
                    <img src="/ui/arrow_top.png" alt="" class="w-[24px]">
                </div>
            </div>
        </div>

        <div class="relative w-[520px] h-[385px] ml-auto flex justify-end items-center player_">
            <!-- <img src="/img/vector.png" alt="" class="absolute w-[318px] right-[200px] top-[5px] z-[1] vector"> -->
            <img src="/img/american-football-player.png" alt="" class="w-[520px] h-[385px] relative z-[2] player">
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .news {
        width: 1440px;
        margin: 50px auto;
    }
}

@media screen and (max-width: 1500px) {
    .news {
        width: 1240px;
        margin: 50px auto;
    }
}

@media screen and (max-width: 1300px) {
    .news {
        width: 1000px;
        height: fit-content;
        margin: 50px auto;
        flex-direction: column;
    }
}

@media screen and (max-width: 1050px) {
    .news {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .news {
        width: 768px;
        gap: 30px;
    }
}

@media screen and (max-width: 920px) {
    .news {
        width: auto;
        margin: 50px 20px;
        padding: 20px 20px 0;
    }
}

@media screen and (max-width: 660px) {
    .news_input {
        margin: 30px auto 0;
        justify-content: center;
    }
}

@media screen and (max-width: 600px) {
    .news{
        margin: 50px 20px 30px;
    }
    .news_input {
        margin: 10px auto 0;
        justify-content: center;
    }

    .input {
        width: auto;
    }

    .sub {
        width: fit-content;
    }

    .input input {
        width: 100%;
    }

    .input div {
        width: 20%;
    }
}

@media screen and (max-width: 560px) {
    .player_ {
        width: auto;
        height: auto;
    }

    .vector {
        width: 278px;
        height: auto;
        right: 120px;
        top: -25px;
    }

    .player {
        width: 400px;
        height: auto;
    }
}

@media screen and (max-width: 490px) {
    .sub{
        font-size: 48px;
    }
}

@media screen and (max-width: 410px) {
    .sub{
        font-size: 36px;
    }

    .input div img{
        width: 16px;
        height: 16px;
    }
}
</style>