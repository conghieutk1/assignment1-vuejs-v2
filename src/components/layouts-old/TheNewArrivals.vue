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
    mounted() {
        console.log('window.location.href', window.location.href);
    },
    data() {
        return {
            buttonName: 'View all',
            urlImage1: require('@/assets/images/a7234235e66d6695d9d7098fc3289872.png'), //  '../assets/images/a7234235e66d6695d9d7098fc3289872.png'
            urlImage2: require('@/assets/images/ff941dde9bc0e54431b8d8fe3182f5e9.png'),
            urlImage3: require('@/assets/images/5fc84f87eeac1062fbe47f49c192d4f2.png'),
            urlImage4: require('@/assets/images/7cc557f42cf1d489f7cc811856b90e9f.png'),
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
