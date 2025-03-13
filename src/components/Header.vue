<template>
    <div class="h-[92px] flex items-center justify-between head">
        <p class="font-[Darkline] text-[32px]">Sport News</p>

        <ul class="flex p-0 gap-[19px] text-[#262626] text-[15px] font-[DMSans] ul_list">
            <li class="text-black font-bold">Home</li>
            <li>Category</li>
            <li>Trending News</li>
            <li>Recent News</li>
            <li>Clubs Ranking</li>
            <li>Sports Article</li>
        </ul>

        <button class="flex items-center bg-[#B8C2CE] pl-[15px] pr-[10px] h-[35px] rounded-[6px] gap-[12px] font-[DMSans] text-[14px] text-white">
            <img src="/ui/search.png" alt="" width="16px" height="16px">
            <p>Search</p>
        </button>

        <button class="hidden menu">
            <img src="/ui/menu.png" alt="">
        </button>
    </div>
</template>

<style scoped>
@media screen and (max-width: 1920px) {
    .head{
        max-width: 1440px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1500px) {
    .head {
        width: 1240px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1300px) {
    .head {
        width: 1000px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 1050px) {
    .head {
        width: 880px;
        margin: 0 auto;
    }
}

@media screen and (max-width: 920px) {
    .head {
        width: 768px;
        margin: 0 auto;
    }

    .ul_list{
        display: none;
    }

    .menu{
        display: block;
        width: 20px;
    }
}

@media screen and (max-width: 800px) {
    .head {
        width: auto;
        margin: 0 20px;
    }

}
</style>