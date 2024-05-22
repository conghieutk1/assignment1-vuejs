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

<style lang="scss">
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
.test-scss {
    margin-top: 500px;
    width: 100%;
    height: 500px;
    .test-scss-01 {
        font-size: 30px;
        border: 1px solid red;
    }
}
</style>
