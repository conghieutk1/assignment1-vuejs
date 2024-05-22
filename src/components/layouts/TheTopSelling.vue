<template>
    <div class="container">
        <div class="title">TOP SELLING</div>
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
</template>
<script>
import BaseButton from '../UI/BaseButton.vue';
import BaseItem from '../UI/BaseItem.vue';
export default {
    data() {
        return {
            buttonName: 'View all',
            urlImage1:
                'https://s3-alpha-sig.figma.com/img/e01f/5d3c/d9029bd465a4c7158689ab1619693014?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=CS6VVx942xweaJzOSk77qavQIsSnTeCKFJ9un2~ioxUHY9EKdTjt4~qePOZWMbkxGl4GEIDB8DN7ldczsw5TsgTexL7B6fkUfwx6HnJ42ug6iG8BsN-rbmTi2aaGF8FN71swFpvyU09e0hWaMuefZr1e85W~qYwtVvtb0dPbPWF~K66s-o1fSnSVkW51ykL3kCR54b-V8xU0kCFbPAezvjDLeTIw0g3Cj9bQO19wY90c8YSUOgdgrOuH~nT5IZc6doU1uJBeKe52LNgaiPAkQ734Is4cQcIs5X4A04o1yJkSxzgtiiGpIzy1PjRtwroGi3OlJzu-sdLQ-j61IgLhOw__',
            urlImage2:
                'https://s3-alpha-sig.figma.com/img/5723/4b01/d5fcac5632cf6823570ca2d1d53d7d73?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=pfC1btfF1RZLzji53iyktw~scoXkxZ8LhcYlDybzn1BR6WaREXQonNV1PESvWjXMPDoUH3fGOMCdEbrlI-U7TzTxoIQRsrM6aa-EcddIoE7Ms9gfHwy9FcKNOLrYWQK7kK9Sy3sEzpMVY59igWYuAclIE9ahvvDXZryR2FsjXXgtXus8negNqh6~Pbneptpwom6szdVijsjCDJrTtG1Aluldgo-rNPJKoMnBGaKDjo4oUang-6GwxnO4nZMFkKi7hJCJLtaf~1UNAzI6a27HFgFcMuTDNvnUUZbRWwY1CiR~dJmK5KhvJxJyeoJ2QM-8YJ4HlQiSpYu37qZonkUf2Q__',
            urlImage3:
                'https://s3-alpha-sig.figma.com/img/8951/5d71/4a66d9ca1401101dee4cc689f8bb5ad2?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=N3uW6eTpMajf2Xkh0dusIQt7AXrxqNYnlK7ekgXtsb4A-tD9rk~kAhD2WLaewyEKhk12LzCTUfCgrE2blOU1ViMcaom2CRi2SDpSoLIQMMGMs8SUpXlbbucGW1-YwmDYTUVv2y4A0-iGbKkTzw7meU6xocHzM8Np63~RCO-MYH14Cfv0hQcBt2BHQPIrSNGaS1jgdWDVyh5yzNzqMI2u7yR-cl1uNKC0-D8DNKq4WrLdFl5xspx3f7aLD9VCsROHUk1eSHSZXFmsGu9KkpfX6AZr7-sPT3Yv0MY2YIFGDkZvsPiSqziCg6Nj~O7HxgIOZq3EFywkH11PB4nBlDEr-A__',
            urlImage4:
                'https://s3-alpha-sig.figma.com/img/f180/c768/08e2ff8a46be56aa933f031aed3abe75?Expires=1716768000&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=oyCs5cchDx4qGB~~HSQF04Cn-WUiTDANxUnKyg~ZRaV2fDQK6dlFteMXYDrzZkOihRAjK8hfYq-GW6Z5fCZRYa9dJX-VbYYNdDP-fRPq09isa16zUTGMQMe2PhtZHwU-qwQdKZJVkSYNbWueBKc3t9p6mdxdF5MPlBZsoZBY0Z1Ri1cF3oq~gbKRV9SzLUWQzXJi0C86lyHWXFbPAV5uKLgmMYGFUehDTTZ7AlxP5Oz4ybHIGWj~oerPyindKnVknmX4iakRurmohcc~mXtJSyp8XChJPapCo764L-ou9HSKzDcx4QWRTvJrkfoLYtpOii8~NrlWItzCa8r78qeyNA__',
            nameImage1: 'Vertical Striped Shirt',
            nameImage2: 'Courage Graphic T-shirt',
            nameImage3: 'Loose Fit Bermuda Shorts',
            nameImage4: 'Faded Skinny Jeans',
            priceImage1: '$212',
            priceImage2: '$145',
            priceImage3: '$80',
            priceImage4: '$210',
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
    margin-bottom: 100px;
}
.title {
    /* margin-top: 72px; */
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
