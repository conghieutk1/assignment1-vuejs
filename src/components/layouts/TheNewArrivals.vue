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
            urlImage1:
                'https://s3-alpha-sig.figma.com/img/d40d/a9a3/a7234235e66d6695d9d7098fc3289872?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=cHnK5m7w639I3Bl8MtSd1WEvKBDNsVl~ubjILULUL-dEKXFsLu3hc5OYhL4F9zs0MF0GEfDhEeakW~8vU7imq5jf0GZVVDHt7GVujj4Rp1s3oSONaqZI5Ixe9y07G4~pr1uoM2F2mYTD~ceH0igLdevjF3yclJZUXsq-pmINnHh66BXuGbGiJbXHa0OBu2hlAlrCYKntJCFPB-k~z9mQ~aHb82hXxLHxrSZDg7WTEXiiTXvPynAG95n4~fhZfA5SApoX2uQ5KzsZc780hMR5T1niVO-RpDmGMnrbVyws5XDZGG8kfoxDoO5~f4m7f7ZmiCDrgaWvbkRoPbhC9fVblg__',
            urlImage2:
                'https://s3-alpha-sig.figma.com/img/769b/9d60/ff941dde9bc0e54431b8d8fe3182f5e9?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=mi9aT-lkwmByLaUCKF~domGRLV4Hx-GVFf~7WorFe1o~alG26Woq-ksWIz9q1MwK-9f7GMyj01AGXNnR~0ICRIHMMClGsvYivmm3KMb9714cY0pb8u1DNOrs~zC3XFrAe1RAeix2eD1MYzF0V8f18g807LczpASh~fWuIbbPaTA6qvflctUkZw3mRvb5~FVeFDX3iqEsdn9fEuaFzGSZpmiVkdP2mAcm0nTtJk1ieeM-OaEg8soQ5Pifsbx0M6VF1P0jcLN7sVePg4-q34zuYa6~QdREfChVAPD3~1avTMYGW5wU37xSJdPb4FGSCXv383Sp7xGSp80LktLhB3tK3A__',
            urlImage3:
                'https://s3-alpha-sig.figma.com/img/bbf4/11c2/5fc84f87eeac1062fbe47f49c192d4f2?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=Wo3YKqHSumtrIAwgYgbv1ILwuzhyBkFn3H3LzDQjR71HHidKU6o8qjhny6PPPrsw6Fq8U2tBy~Dq-Z1PbY9TKTJTVhssIW9xSG6mhZOSV3oeUsMyy67MlCru-YA0~Itz-YvYLLR5~lEt09oO3siyleT-~G8USSwJfkWstkEscsvIc4erLvvdGHmJCTGXKbxRxKFvz9uuidXxwbKDaFnwWsxA-AbBuV6HjIcuTFdREUnnFH14xfOcGknHG1FPu3YOVg07rutZmCIHC~rvK2rUUQkmaipVj0LcE7R1-TRqX64aOcSM5Sz2My6VK607nLnsVIuTtFEhmmO~gish~iT~2g__',
            urlImage4:
                'https://s3-alpha-sig.figma.com/img/3457/42c2/7cc557f42cf1d489f7cc811856b90e9f?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W7R16BkakmKIbof-rWg0Fi1DzW2q87CyDgdpi469brBOyPtXdvilG005Bv5k~WtEF~B5ozXAfQT5x25gzhvQ2xk7-N7zkQ9~IyPZjh17re1bqwCDmVapMNeFWfbU~2zdaVqrnzTzkW8g0ER7YZt-y~o2Oe~D4jfHxFS5c2FBGbESdBikqnqJMGn~VKzYmrTxta1R8uOPI3-6m8~qcONIGIYktpTWEH692XXnFQBilQPdj1BGBaS1PZDyE9T3A1Dhou2WSvW7XwEwuH-JgI7MK-HXXFxqNTaeqBWUf~C6YkhCjrGTUdz9HuylP1gaQuMpnrud7DnnXFrSViFOYCBeMw__',
            nameImage1: 'T-shirt with Tape Details',
            nameImage2: 'Skinny Fit Jeans',
            nameImage3: 'Checkered Shirt',
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
    overflow-x: auto; /* Tạo thanh trượt ngang khi cần thiết */
    max-width: 100%;
    gap: 10px;
    margin-bottom: 36px;
}
@media (max-width: 768px) {
    .container {
        display: grid;
        justify-items: center;
        padding: 0px 25px;
    }
    .line-separation {
        height: 1px;
        background-color: #000000;
        opacity: 10%;
        margin: 50px 25px;
    }
}
</style>
