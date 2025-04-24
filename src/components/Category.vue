<template>
    <section id="category" class="mx-[135px] my-[80px] flex flex-col gap-[24px] category">
        <p class="font-[Kanit-Medium] text-[28px]">Category</p>

        <div class="flex justify-between categories">
            <div class="flex gap-[30px] flex-col w-[270px]">
                <div class="bg-[#EBEEF3] rounded-[6px] flex justify-center items-center h-[116px]">
                    <p
                        class="font-[Kanit-Bold] text-[37px] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text uppercase">
                        Football</p>
                </div>
                <img src="/img/football.png" width="270px" alt="">
            </div>

            <div class="flex gap-[30px] flex-col-reverse w-[270px]">
                <div class="bg-[#EBEEF3] rounded-[6px] flex justify-center items-center h-[169px]">
                    <p
                        class="font-[Kanit-Bold] text-[37px] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text uppercase w-[210px] leading-[95%] text-center">
                        Bascket ball</p>
                </div>
                <img src="/img/basketball.png" alt="" class="w-[270px] h-[235px]">
            </div>

            <div class="flex gap-[30px] flex-col w-[270px]">
                <div class="bg-[#EBEEF3] rounded-[6px] flex justify-center items-center h-[116px]">
                    <p
                        class="font-[Kanit-Bold] text-[37px] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text uppercase ">
                        Car sport</p>
                </div>
                <img src="/img/sportcar.png" alt="" class="w-[270px] h-[286px]">
            </div>

            <div class="flex gap-[30px] flex-col-reverse w-[270px]">
                <div class="bg-[#EBEEF3] rounded-[6px] flex justify-center items-center h-[116px]">
                    <p
                        class="font-[Kanit-Bold] text-[37px] bg-gradient-to-b from-[#262626] to-[#B8C2CE] text-transparent bg-clip-text uppercase w-[210px] leading-[95%] text-center">
                        Table Tennis</p>
                </div>
                <div class="bg-black w-[270px] h-[286px] rounded-[6px] flex justify-center items-end pb-[42px]">
                    <img src="/img/ping-pong.png" width="270px" alt="" class="rounded-[6px]">
                </div>
            </div>
        </div>
    </section>


</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .category{
        width: 1440px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1500px) {
    .category {
        width: 1240px;
        margin: 80px auto;
    }
}

@media screen and (max-width: 1300px) {
    .category {
        width: 1000px;
        margin: 80px auto;
    }

    .categories{
        flex-wrap: wrap;
        gap: 30px;
    }
}

@media screen and (max-width: 1050px) {
    .category {
        width: 880px;
    }
}

@media screen and (max-width: 920px) {
    .category {
        width: 768px;
    }
}

@media screen and (max-width: 800px) {
    .category {
        width: auto;
        margin: 80px 20px;
    }
}

@media screen and (max-width: 610px) {
    .categories{
        justify-content: center;
    }
}

@media screen and (max-width: 600px) {
    .category {
        margin: 130px 20px 80px;
    }
}
</style>