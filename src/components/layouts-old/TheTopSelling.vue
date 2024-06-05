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
            urlImage1: require('@/assets/images/d9029bd465a4c7158689ab1619693014.png'), //  '../assets/images/a7234235e66d6695d9d7098fc3289872.png'
            urlImage2: require('@/assets/images/d5fcac5632cf6823570ca2d1d53d7d73.png'),
            urlImage3: require('@/assets/images/4a66d9ca1401101dee4cc689f8bb5ad2.png'),
            urlImage4: require('@/assets/images/08e2ff8a46be56aa933f031aed3abe75.png'),
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
