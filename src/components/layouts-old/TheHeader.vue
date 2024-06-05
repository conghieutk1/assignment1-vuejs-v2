<template>
    <div>
        <link
            rel="stylesheet"
            href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0"
        />
        <div class="transition" v-if="isShowDiscount">
            <div class="info-discount">
                Sign up and get 20% off to your first order.
            </div>
            <a href="#"> Sign Up Now</a>
            <span
                class="material-symbols-outlined close-btn"
                @click="closeDiscount"
            >
                close
            </span>
        </div>
        <div class="header-container">
            <div class="nav-btn">
                <svg
                    width="20"
                    height="16"
                    viewBox="0 0 20 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        d="M19.375 8C19.375 8.29837 19.2565 8.58452 19.0455 8.79549C18.8345 9.00647 18.5484 9.125 18.25 9.125H1.75C1.45163 9.125 1.16548 9.00647 0.954505 8.79549C0.743526 8.58452 0.625 8.29837 0.625 8C0.625 7.70163 0.743526 7.41548 0.954505 7.2045C1.16548 6.99353 1.45163 6.875 1.75 6.875H18.25C18.5484 6.875 18.8345 6.99353 19.0455 7.2045C19.2565 7.41548 19.375 7.70163 19.375 8ZM1.75 3.125H18.25C18.5484 3.125 18.8345 3.00647 19.0455 2.7955C19.2565 2.58452 19.375 2.29837 19.375 2C19.375 1.70163 19.2565 1.41548 19.0455 1.2045C18.8345 0.993526 18.5484 0.875 18.25 0.875H1.75C1.45163 0.875 1.16548 0.993526 0.954505 1.2045C0.743526 1.41548 0.625 1.70163 0.625 2C0.625 2.29837 0.743526 2.58452 0.954505 2.7955C1.16548 3.00647 1.45163 3.125 1.75 3.125ZM18.25 12.875H1.75C1.45163 12.875 1.16548 12.9935 0.954505 13.2045C0.743526 13.4155 0.625 13.7016 0.625 14C0.625 14.2984 0.743526 14.5845 0.954505 14.7955C1.16548 15.0065 1.45163 15.125 1.75 15.125H18.25C18.5484 15.125 18.8345 15.0065 19.0455 14.7955C19.2565 14.5845 19.375 14.2984 19.375 14C19.375 13.7016 19.2565 13.4155 19.0455 13.2045C18.8345 12.9935 18.5484 12.875 18.25 12.875Z"
                        fill="black"
                    />
                </svg>
            </div>
            <div class="logo">SHOP.CO</div>
            <div class="nav-header">
                <BaseButtonHeader :nameTab="firstTab" />
                <BaseButtonHeader :nameTab="secondTab" />
                <BaseButtonHeader :nameTab="thirdTab" />
                <BaseButtonHeader :nameTab="fourTab" />
            </div>
            <span class="material-symbols-outlined search-icon-mobile">
                search
            </span>
            <div class="nav-search">
                <span class="material-symbols-outlined search-icon">
                    search
                </span>
                <input
                    class="text-search"
                    placeholder="Search for products..."
                />
            </div>
            <div class="cart-and-person">
                <button class="effect-click">
                    <span class="material-symbols-outlined icon-cart">
                        shopping_cart
                    </span>
                </button>
                <button class="effect-click">
                    <span class="material-symbols-outlined icon-account">
                        account_circle
                    </span>
                </button>
            </div>
        </div>
    </div>
</template>

<script>
import BaseButtonHeader from '../UI/ButtonCollection/BaseButtonHeader.vue';
export default {
    data() {
        return {
            isShowDiscount: true,
            firstTab: 'Shop',
            secondTab: 'One Sale',
            thirdTab: 'New Arrivals',
            fourTab: 'Brands',
        };
    },
    methods: {
        closeDiscount() {
            this.isShowDiscount = false;
        },
    },
    components: {
        BaseButtonHeader,
    },
};
</script>

<style lang="scss" scoped>
a {
    &:hover {
        color: #ffffffe8;
    }
}
.icon-account,
.icon-cart {
    margin: auto;
    display: flex;
    justify-content: center;
}
.effect-click {
    background: white;
    height: 44px;
    width: 44px;
    border: none;
    outline: none;
    cursor: pointer;
    border-radius: 50%;
    &:hover {
        background: #f2f0f1;
    }
}

.transition {
    width: 100%;
    height: 38px;
    background-color: black;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
}
.info-discount {
    font-size: 14px;
    font-weight: 400;
    line-height: 18.9px;
    text-align: left;
    font-family: 'Satoshi', sans-serif;
}
a {
    color: white;
    font-size: 14px;
    font-weight: 500;
    line-height: 18.9px;
    text-align: left;
    margin-left: 3px;
}
.close-btn {
    position: absolute;
    right: 0;
    cursor: pointer;
    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
    margin-right: 300px;
    justify-items: right;
}
.header-container {
    width: 100%;
    height: 96px;
    /* border: 1px solid blue; */
    display: flex;
    justify-content: left;
    align-items: center;
    padding: 0px 300px;
}
.logo {
    font-family: 'Integral CF', sans-serif;
    font-size: 32px;
    letter-spacing: -0.09em;
    font-weight: 800;
    line-height: 38.4px;
    text-align: left;
    margin-right: 50px;
    cursor: pointer;
}
.nav-header {
    display: flex;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 21.6px;
    text-align: left;
    gap: 10px;
    margin-right: 40px;
}
.nav-search {
    width: 577px;
    height: 48px;
    border-radius: 25px;
    display: flex;
    justify-items: center;
    align-items: center;
    background-color: #f0f0f0;
    /* padding-top: 12px; */
    padding-left: 20px;
    padding-right: 30px;
    margin-left: auto;
    margin-right: 20px;
}
.text-search {
    border: 1px solid transparent;
    width: 90%;
    padding: 5px 0px;
    outline: none;
    background-color: #f0f0f0;
    margin-left: 12px;
    opacity: 60%;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 21.6px;
    text-align: left;
}
.search-icon {
    opacity: 100%;
}
.cart-and-person {
    /* width: 577px;
    height: 48px; */
    display: flex;
    gap: 15px;
    justify-items: center;
    margin-left: 15px;
    /* margin-left: auto; */
    /* align-items: right; */
    /* border: 1px solid red; */
}
@media (max-width: 1600px) {
    .header-container {
        padding: 0px 100px;
    }
    .close-btn {
        margin-right: 100px;
    }
}
@media (max-width: 1080px) {
    .header-container {
        padding: 0px 40px !important;
    }
    .nav-search {
        display: none;
    }
    .search-icon-mobile {
        margin-left: auto;
    }
    .close-btn {
        margin-right: 40px;
    }
}

@media (min-width: 1080px) {
    .nav-btn {
        display: none;
    }
    .search-icon-mobile {
        display: none;
    }
}
@media (max-width: 768px) {
    .header-container {
        padding: 0px 25px !important;
    }
    .nav-btn {
        display: flex;
        justify-items: center;
        align-items: center;
        margin-right: 15px;
    }
    .close-btn {
        display: none;
    }
    .nav-header {
        display: none;
    }
    .search-icon-mobile {
        margin-left: auto;
    }

    .text-search {
        display: none;
    }
}

@media (min-width: 768px) {
    .nav-btn {
        display: none;
    }
}
</style>
