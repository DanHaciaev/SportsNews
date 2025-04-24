<template>
    <div
        class="h-[92px] flex items-center justify-between fixed top-0 left-0 right-0 z-[50] bg-[rgb(255,255,255,0.5)] backdrop-blur-md head">
        <p @click="scrollToSection('home')" class="font-[Darkline] text-[32px] cursor-pointer">
            Sport News
        </p>

        <ul class="flex p-0 gap-[19px] text-[#262626] text-[15px] font-[DMSans] ul_list">
            <li @click="scrollToSection('home')" :class="activeSection === 'home' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Home
            </li>
            <li @click="scrollToSection('category')" :class="activeSection === 'category' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Category
            </li>
            <li @click="scrollToSection('trending')" :class="activeSection === 'trending' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Trending News
            </li>
            <li @click="scrollToSection('recent')" :class="activeSection === 'recent' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Recent News
            </li>
            <li @click="scrollToSection('ranking')" :class="activeSection === 'ranking' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Clubs Ranking
            </li>
            <li @click="scrollToSection('sports')" :class="activeSection === 'sports' ? 'text-black font-bold' : ''"
                class="cursor-pointer">
                Sports Article
            </li>
        </ul>


        <button
            class="flex items-center bg-[#B8C2CE] pl-[15px] pr-[10px] h-[35px] rounded-[6px] gap-[12px] font-[DMSans] text-[14px] text-white">
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
    .head {
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

    .ul_list {
        display: none;
    }

    .menu {
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

<script setup>
import { ref, onMounted } from 'vue';

const activeSection = ref('home'); // по умолчанию активен Home

const scrollToSection = (id) => {
  const el = document.getElementById(id);
  if (el) {
    const yOffset = -92;
    const y = el.getBoundingClientRect().top + window.pageYOffset + yOffset;
    window.scrollTo({ top: y, behavior: 'smooth' });
  }
  activeSection.value = id; // 👈 установить активную секцию
};

const sections = ['home', 'category', 'trending', 'recent', 'ranking', 'sports'];

const observer = new IntersectionObserver(
  (entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        // Устанавливаем активную секцию, если она видна
        activeSection.value = entry.target.id;
      }
    });
  },
  {
    rootMargin: '-50% 0px', // секция считается видимой, когда она на 50% появляется в поле зрения
  }
);

onMounted(() => {
  // Наблюдаем за всеми секциями
  sections.forEach(section => {
    const el = document.getElementById(section);
    if (el) {
      observer.observe(el);
    }
  });
});
</script>

