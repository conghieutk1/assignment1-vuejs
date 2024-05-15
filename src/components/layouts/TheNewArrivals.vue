<template>
    <div class="container">
        <div class="title">NEW ARRIVALS</div>
        <div class="list-items">
            <BaseItem
                :dynamicImage="urlImage1"
                :itemName="nameImage1"
                :itemPrice="priceImage1"
            />
            <BaseItem
                :dynamicImage="urlImage2"
                :itemName="nameImage2"
                :itemPrice="priceImage2"
            />
            <BaseItem
                :dynamicImage="urlImage3"
                :itemName="nameImage3"
                :itemPrice="priceImage3"
            />
            <BaseItem
                :dynamicImage="urlImage4"
                :itemName="nameImage4"
                :itemPrice="priceImage4"
            />
        </div>
        <BaseButton :buttonName="buttonName" />
    </div>
    <div class="line-separation"></div>
</template>
<script>
import BaseButton from '../UI/BaseButton.vue';
import BaseItem from '../UI/BaseItem.vue';
export default {
    data() {
        return {
            buttonName: 'View all',
            urlImage1: '../../assets/items/image 7.png',
            urlImage2: '../../assets/items/image 8.png',
            urlImage3: '../../assets/items/image 9.png',
            urlImage4: '../../assets/items/image 10.png',
            nameImage1: 'T-shirt with Tape Details',
            nameImage2: 'Skinny Fit Jeans',
            nameImage3: 'Checkered',
            nameImage4: 'Sleeve Striped T-shirt',
            priceImage1: '$120',
            priceImage2: '$240',
            priceImage3: '$180',
            priceImage4: '$130',
        };
    },
    components: { BaseButton, BaseItem },
};
</script>
<style scoped>
.container {
    display: grid;
    justify-items: center;
    padding: 0px 100px;
}
.line-separation {
    height: 1px;
    background-color: #000000;
    opacity: 10%;
    margin: 80px 100px;
}
.title {
    margin-top: 72px;
    font-family: 'Integral CF', sans-serif;
    letter-spacing: -0.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
}
.list-items {
    margin-top: 52px;
    display: flex;
    gap: 10px;
    margin-bottom: 36px;
}
</style>
