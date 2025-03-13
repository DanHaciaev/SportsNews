<template>
    <div class="flex justify-between bottom">
        <div class="flex items-center gap-[16px]">
            <div class="bg-black w-[44px] h-[45px] flex items-center justify-center rounded-[4px]">
                <img src="/img/facebook.png" alt="" class="w-[18px]">
            </div>
            <div class="bg-black w-[44px] h-[45px] flex items-center justify-center rounded-[4px]">
                <img src="/img/instagram.png" alt="" class="w-[28px]">
            </div>
            <div class="bg-black w-[44px] h-[45px] flex items-center justify-center rounded-[4px]">
                <img src="/img/twitter.png" alt="" class="w-[26px]">
            </div>
        </div>

        <div class="flex w-[470px] items-center justify-between next">
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

<style>
@media screen and (max-width: 1920px) {
    .bottom {
        width: 1440px;
        margin: 50px auto;
    }
}

@media screen and (max-width: 1500px) {
    .bottom {
        width: 1240px;
    }
}

@media screen and (max-width: 1300px) {
    .bottom {
        width: 1000px;
    }
}

@media screen and (max-width: 1050px) {
    .bottom {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .bottom {
        width: 768px;
    }
}

@media screen and (max-width: 800px) {
    .bottom {
        width: auto;
        margin: 50px 20px;
    }
}

@media screen and (max-width: 800px) {
    .bottom {
        flex-direction: column-reverse;
        gap: 24px;
    }

    .next {
        margin-left: auto;

    }
}

@media screen and (max-width: 600px) {
    .bottom {
        margin: 0 20px 50px;
    }

    .next {
        width: auto;
        gap: 24px;
    }

    .next button {
        width: 50px;
        height: 30px;
    }

    .next div:nth-child(1) {
        width: 25px;
    }
}
</style>