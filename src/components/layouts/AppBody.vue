<template>
    <AppBanner />
    <AppBannerBrands />
    <AppProductsList :title="titleArrival" :listItems="listProductArrivals" />
    <AppProductsList
        :title="titleTopSelling"
        :listItems="listProductTopSelling"
    />
    <AppItemCategory />
    <AppFeedback />
</template>
<script>
import AppBanner from '../layouts/body/AppBanner.vue';
import AppBannerBrands from '../layouts/body/AppBannerBrands.vue';
import AppProductsList from '../layouts/body/AppProductsList.vue';
import AppItemCategory from '../layouts/body/AppItemCategory.vue';
import AppFeedback from '../layouts/body/AppFeedback.vue';

export default {
    data() {
        return {
            titleArrival: 'NEW ARRIVALS',
            titleTopSelling: 'TOP SELLING',
            listProductArrivals: [
                {
                    urlImage: require('@/assets/images/a7234235e66d6695d9d7098fc3289872.png'),
                    nameProduct: 'T-shirt with Tape Details',
                    price: '$120',
                    rating: '4.5',
                    originPrice: '',
                    percentDiscount: '',
                },
                {
                    urlImage: require('@/assets/images/ff941dde9bc0e54431b8d8fe3182f5e9.png'),
                    nameProduct: 'Skinny Fit Jeans',
                    price: '$240',
                    rating: '4.5',
                    originPrice: '$260',
                    percentDiscount: '-20%',
                },
                {
                    urlImage: require('@/assets/images/5fc84f87eeac1062fbe47f49c192d4f2.png'),
                    nameProduct: 'Checkered Shirt',
                    price: '$180',
                    rating: '4.5',
                    originPrice: '',
                    percentDiscount: '',
                },
                {
                    urlImage: require('@/assets/images/7cc557f42cf1d489f7cc811856b90e9f.png'),
                    nameProduct: 'Sleeve Striped T-shirt',
                    price: '$130',
                    rating: '4.5',
                    originPrice: '$160',
                    percentDiscount: '-30%',
                },
            ],
            listProductTopSelling: [
                {
                    urlImage: require('@/assets/images/d9029bd465a4c7158689ab1619693014.png'),
                    nameProduct: 'Vertical Striped Shirt',
                    price: '$212',
                    rating: '4.5',
                    originPrice: '232',
                    percentDiscount: '-20%',
                },
                {
                    urlImage: require('@/assets/images/7cc557f42cf1d489f7cc811856b90e9f.png'),
                    nameProduct: 'Courage Graphic T-shirt',
                    price: '$145',
                    rating: '4.5',
                    originPrice: '',
                    percentDiscount: '',
                },
                {
                    urlImage: require('@/assets/images/4a66d9ca1401101dee4cc689f8bb5ad2.png'),
                    nameProduct: 'Loose Fit Bermuda Shorts',
                    price: '$80',
                    rating: '4.5',
                    originPrice: '',
                    percentDiscount: '',
                },
                {
                    urlImage: require('@/assets/images/08e2ff8a46be56aa933f031aed3abe75.png'),
                    nameProduct: 'Faded Skinny Jeans',
                    price: '$210',
                    rating: '4.5',
                    originPrice: '',
                    percentDiscount: '',
                },
            ],
        };
    },
    components: {
        AppBanner,
        AppBannerBrands,
        AppProductsList,
        AppItemCategory,
        AppFeedback,
    },
};
</script>
<style lang="scss" scoped>
@import '../../assets/styles/global.scss';
</style>
