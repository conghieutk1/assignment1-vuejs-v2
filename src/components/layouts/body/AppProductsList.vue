<template>
    <div class="list-items-container">
        <div class="wrapper">
            <div class="title">{{ title }}</div>
            <div class="list-items">
                <BaseItem
                    v-for="(item, index) in listItems"
                    :key="index"
                    :itemImage="item.urlImage"
                    :itemName="item.nameProduct"
                    :itemPrice="item.price"
                    :itemOriginPrice="item.originPrice"
                    :itemPercentDiscount="item.percentDiscount"
                />
            </div>
            <BaseButton :buttonName="buttonName" />
        </div>
    </div>
</template>
<script>
import BaseButton from '../../ui/body/button/BaseButton.vue';
import BaseItem from '../../ui/body/item/BaseItem.vue';
export default {
    props: ['title', 'listItems'],

    data() {
        return {
            buttonName: 'View all',
        };
    },
    components: { BaseItem, BaseButton },
};
</script>
<style lang="scss" scoped>
@import '../../../assets/styles/global.scss';
.list-items-container {
    display: grid;
    justify-items: center;
    padding: 0 100px;

    @include medium-screen {
        padding: 0 50px;
    }

    @include tablet {
        padding: 0 50px;
    }

    @include mobile {
        padding: 0 25px;
    }

    .wrapper {
        height: 100%;
        overflow-x: auto;
        width: 100%;
        margin: 0 auto;
        justify-content: center;
        max-width: 1440px;
        padding-bottom: 50px;
        border-bottom: 1px solid #0000002f;
        .title {
            margin-top: 72px;
            font-family: 'Integral CF', sans-serif;
            letter-spacing: -0.07em;
            font-size: 48px;
            font-weight: 800;
            line-height: 57.6px;
            text-align: center;

            @include tablet {
                margin-top: 45px;
                font-size: 37px;
            }
        }

        .list-items {
            margin-top: 52px;
            display: flex;
            overflow-x: auto;
            gap: 10px;
            margin-bottom: 36px;
            margin: 52px 0px 36px 0px;
            justify-content: space-between;

            @include medium-screen {
                margin: 52px 0px 36px 0px;
            }

            @include tablet {
                margin: 52px 0px 36px 0px;
            }

            @include mobile {
                margin: 52px 0px 36px 0px;
            }
        }
    }
}
</style>
