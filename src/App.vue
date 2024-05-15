<template>
    <div>
        <TheHeader />
        <TheIntro />
        <TheNewArrivals />

        <TheTopSelling />
        <TheItemCategory />
        <TheFeetback />
        <TheFooter />
    </div>
</template>

<script>
import TheHeader from './components/layouts/TheHeader.vue';
import TheIntro from './components/layouts/TheIntro.vue';
import TheNewArrivals from './components/layouts/TheNewArrivals.vue';
import TheTopSelling from './components/layouts/TheTopSelling.vue';
import TheItemCategory from './components/layouts/TheItemCategory.vue';
import TheFeetback from './components/layouts/TheFeetback.vue';
import TheFooter from './components/layouts/TheFooter.vue';
export default {
    components: {
        TheHeader,
        TheIntro,
        TheNewArrivals,
        TheTopSelling,
        TheItemCategory,
        TheFeetback,
        TheFooter,
    },
    data() {
        return {};
    },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
    box-sizing: border-box;
}

html {
    font-family: 'Roboto', sans-serif;
}

body {
    margin: 0;
}
.a {
    height: 500px;
}
.line-separation {
    height: 1px;
    background-color: #000000;
    opacity: 10%;
    margin: 80px 100px;
}
</style>
