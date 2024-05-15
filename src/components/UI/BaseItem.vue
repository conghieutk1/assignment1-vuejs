<template>
    <div>
        <div
            class="item-image"
            :style="{ backgroundImage: 'url(' + dynamicImage + ')' }"
        ></div>
        <div class="item-name">{{ itemName }}</div>
        <div class="item-rate"></div>
        <div class="item-price">{{ itemPrice }}</div>
    </div>
</template>
<script>
export default {
    props: ['buttonName', 'dynamicImage', 'itemName', 'itemPrice'],
};
</script>
<style scoped>
.item-image {
    width: 295px;
    height: 298px;
    background-size: cover;
    background-image: url('../../assets/items/image 7.png');
    border-radius: 15px;
    display: block;
    align-content: center;
    /* justify-items: center; */
    /* align-items: center; */
    /* width: 100%; */
}
.item-name {
    margin-top: 10px;
    font-family: 'Satoshi', sans-serif;
    font-size: 15px;
    font-weight: 700;
    line-height: 27px;
    text-align: left;
}
.item-rate {
    margin-top: 5px;
}
.item-price {
    font-family: 'Satoshi', sans-serif;
    margin-top: 5px;
    font-size: 24px;
    font-weight: 700;
    line-height: 32.4px;
    text-align: left;
}
</style>
