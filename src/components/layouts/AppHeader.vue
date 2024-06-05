<template>
    <div class="container">
        <div class="transition" v-if="isShowDiscount">
            <div class="wrapper">
                <div class="space"></div>
                <div class="info-discount">
                    Sign up and get 20% off to your first order.
                    <a href="#"> Sign Up Now</a>
                </div>

                <span
                    class="material-symbols-outlined close-btn"
                    @click="closeDiscount"
                >
                    close
                </span>
            </div>
        </div>
        <div class="header-container">
            <div class="wrapper">
                <div class="nav-btn">
                    <span class="material-symbols-outlined"> menu </span>
                    <div class="logo">SHOP.CO</div>
                </div>

                <div class="nav-header">
                    <BaseButtonHeader :nameTab="firstTab" />
                    <BaseButtonHeader :nameTab="secondTab" />
                    <BaseButtonHeader :nameTab="thirdTab" />
                    <BaseButtonHeader :nameTab="fourTab" />
                </div>

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
    </div>
</template>

<script>
import BaseButtonHeader from '../ui/headerbar/BaseButtonHeader.vue';
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
    components: { BaseButtonHeader },
};
</script>

<style lang="scss" scoped>
@import '../../assets/styles/global.scss';
.container {
    .transition {
        width: 100%;
        height: 38px;
        background-color: black;
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 0px 100px;
        @include medium-screen {
            padding: 0px 50px;
        }
        @include tablet {
            padding: 0px 50px;
        }
        @include mobile {
            padding: 0px 25px;
        }
        .wrapper {
            display: flex;
            justify-content: space-between;
            max-width: 1440px;
            width: 100%;
            // margin: 0 auto;
            .info-discount {
                font-size: 14px;
                font-weight: 100;
                align-content: center;
                margin: 0 auto;
                @include mobile {
                    font-size: 12px;
                }
                a {
                    color: white;
                    font-size: 14px;
                    font-weight: 500;
                    margin-left: 3px;
                    &:hover {
                        color: #ffffffe8;
                    }
                    @include mobile {
                        font-size: 12px;
                    }
                }
            }
            .space {
                width: 20px;
                @include mobile {
                    display: none;
                }
            }
            .close-btn {
                width: 20px;
                cursor: pointer;
                font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0,
                    'opsz' 24;
                display: flex;
                justify-items: right;
                // margin-left: auto;
                @include mobile {
                    display: none;
                }
            }
        }
    }
    .header-container {
        width: 100%;
        height: 96px;
        // border: 1px solid blue;
        background-color: white;
        padding: 0px 100px;
        @include medium-screen {
            padding: 0px 50px;
        }
        @include tablet {
            padding: 0px 50px;
        }
        @include mobile {
            padding: 0px 25px;
        }
        .wrapper {
            height: 96px;
            display: flex;
            max-width: 1440px;
            // border: 1px solid red;
            // justify-content: space-between;
            align-items: center;
            margin: 0 auto;
            .nav-btn {
                display: flex;
                gap: 20px;
                span,
                .logo {
                    margin: auto 0px;
                }
                .logo {
                    font-family: 'Integral CF', sans-serif;
                    font-size: 32px;
                    letter-spacing: -0.09em;
                    font-weight: 800;
                    cursor: pointer;
                }
                span {
                    font-weight: bold;
                    font-size: 40px;
                    display: none;
                    @include medium-screen {
                        display: none;
                    }
                    @include tablet {
                        display: none;
                    }
                    @include mobile {
                        display: block;
                    }
                }
            }
            .nav-header {
                margin-left: 20px;
                width: 100%;
                margin-right: auto;
                min-width: 370px;
                @include mobile {
                    display: none;
                }
            }
            .nav-search {
                width: 100%;
                height: 48px;
                border-radius: 25px;
                display: flex;
                justify-items: center;
                align-items: center;
                background-color: #f0f0f0;
                padding-left: 20px;
                padding-right: 20px;
                margin-left: auto;

                @include tablet {
                    display: none;
                }
                @include mobile {
                    display: none;
                }

                .text-search {
                    border: 1px solid transparent;
                    width: 90%;
                    padding: 5px 0px;
                    outline: none;
                    background-color: #f0f0f0;
                    margin-left: 12px;
                    opacity: 60%;
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 21.6px;
                    text-align: left;
                }
            }
            .cart-and-person {
                @include mobile {
                    margin-left: auto;
                }
                margin-left: 30px;
                display: flex;
                gap: 15px;
                justify-items: center;
                // margin-left: auto;

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
                    .icon-account,
                    .icon-cart {
                        font-size: 30px;
                        margin: auto;
                        display: flex;
                        justify-content: center;
                        font-weight: bold;
                    }
                }
            }
        }
    }
}
</style>
