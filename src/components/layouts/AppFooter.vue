<template>
    <div class="footer-container">
        <div class="wrapper">
            <div class="wrapper-staytoupdate">
                <div class="stay-uptodate">
                    <div class="text-uptodate">
                        STAY UPTO DATE ABOUT OUR LATEST OFFERS
                    </div>
                    <div class="get-infor">
                        <div class="box-enter-email">
                            <span class="material-symbols-outlined">
                                mail
                            </span>

                            <input
                                class="input-email"
                                placeholder="Enter your email address"
                            />
                        </div>
                        <button>Subscribe to Newsletter</button>
                    </div>
                </div>
            </div>
            <div class="contact-list">
                <div class="about-container">
                    <div class="mess">
                        <div class="logo">SHOP.CO</div>
                        <p class="common-text">
                            We have clothes that suits your style and which
                            you’re proud to wear. From women to men.
                        </p>
                    </div>

                    <div class="menu">
                        <div class="about-title">COMPANY</div>
                        <div class="common-text">About</div>
                        <div class="common-text">Features</div>
                        <div class="common-text">Works</div>
                        <div class="common-text">Carrer</div>
                    </div>
                    <div class="menu">
                        <div class="about-title">HELP</div>
                        <div class="common-text">Customer Support</div>
                        <div class="common-text">Delivery Details</div>
                        <div class="common-text">Terms and Conditions</div>
                        <div class="common-text">Privacy policy</div>
                    </div>
                    <div class="menu">
                        <div class="about-title">F A Q</div>
                        <div class="common-text">Account</div>
                        <div class="common-text">Manage Deliveries</div>
                        <div class="common-text">Orders</div>
                        <div class="common-text">Payments</div>
                    </div>
                    <div class="menu">
                        <div class="about-title">RESOURCES</div>
                        <div class="common-text">Free eBooks</div>
                        <div class="common-text">Development Tutorial</div>
                        <div class="common-text">How to - Blog</div>
                        <div class="common-text">Youtube Playlist</div>
                    </div>
                </div>
                <div class="line-separation"></div>
                <div class="list-pay">
                    <div style="color: black; opacity: 60%">
                        Shop.co © 2000-2023, All Rights Reserved
                    </div>
                    <div class="list-pay-2">
                        <img src="../../assets/items/Badge.svg" />
                        <img src="../../assets/items/Badge (1).svg" />
                        <img src="../../assets/items/Badge (2).svg" />
                        <img src="../../assets/items/Badge (3).svg" />
                        <img src="../../assets/items/Badge (4).svg" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {};
    },

    components: {},
};
</script>

<style lang="scss" scoped>
@import '../../assets/styles/global.scss';
.footer-container {
    height: 600px;
    @include medium-screen {
        height: 600px;
    }

    @include tablet {
        height: 700px;
    }

    @include mobile {
        height: 1100px;
    }
    .wrapper {
        width: 100%;
        height: fit-content;
        /* background-color: #f0f0f0; */
        /* opacity: 10%; */
        background-color: white;
        height: 100%;
        margin: 0px auto;

        .wrapper-staytoupdate {
            // padding: 0 100px;
            margin: 0 auto;
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
            .stay-uptodate {
                max-width: 1440px;
                margin: 0px auto;
                height: fit-content;
                border-radius: 20px;
                color: white;
                background-color: black;
                z-index: 2;
                position: relative;
                display: flex;
                @include tablet {
                    flex-direction: column;
                }

                @include mobile {
                }
                // max-width: 1340px;
                .text-uptodate {
                    max-width: 550px;
                    font-size: 40px;
                    font-family: 'Integral CF', sans-serif;
                    letter-spacing: -0.07em;
                    font-weight: 800;
                    line-height: 40px;
                    text-align: left;
                    align-content: center;
                    /* margin-left: 50px; */
                    padding: 0px 50px;
                    @include tablet {
                        margin-top: 20px;
                        max-width: 1000px;
                        text-align: center;
                    }
                }
                .get-infor {
                    display: flex;
                    /* border: 1px solid red; */
                    flex-direction: column;
                    margin: 35px 50px;
                    margin-left: auto;
                    @include tablet {
                        margin: 35px 50px;
                    }
                    /* padding: 0px 30px 0px 250px; */
                    gap: 10px;
                    /* display: grid; */
                    .box-enter-email {
                        padding: 0 100px;
                        height: 48px;
                        width: 100%;
                        // min-width: 350px;
                        border-radius: 30px;
                        outline: none;
                        display: flex;
                        justify-items: center;
                        align-items: center;
                        background-color: #ffffff;
                        /* padding-top: 12px; */
                        gap: 10px;
                        padding-left: 20px;
                        // margin-left: auto;
                        @include tablet {
                            // width: 500px;
                            text-align: center;
                            margin: 0 auto;
                        }
                        .input-email {
                            height: 48px;
                            width: 100%;
                            // max-width: 350px;
                            border-radius: 30px;
                            border: 1px solid transparent;
                            outline: none;
                            font-family: 'Satoshi';
                            background-color: #ffffff;
                        }
                        .material-symbols-outlined {
                            color: #000;
                            opacity: 60%;
                            font-variation-settings: 'FILL' 0, 'wght' 400,
                                'GRAD' 0, 'opsz' 24;
                            justify-items: right;
                        }
                    }

                    button {
                        height: 48px;
                        border-radius: 30px;
                        outline: none;
                        font-family: 'Satoshi';
                        font-size: 16px;
                        font-weight: 500;
                        line-height: 21.6px;
                        text-align: center;
                        background-color: #ffffff;
                        color: #000000;
                        cursor: pointer;
                        width: 100%;
                        // max-width: 350px;
                        // margin-left: auto;
                    }
                }
            }
        }

        .contact-list {
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
            background-color: #f0f0f0;
            position: absolute;
            margin-top: -90px;
            width: 100%;
            height: 100%;
            z-index: 1;
            .about-container {
                // border-bottom: 1px solid #0000001a;
                margin: 0 auto;
                max-width: 1440px;
                // height: 350px;
                width: 100%;
                // padding: 147px 0px;
                padding-top: 147px;
                display: flex;
                justify-content: space-between;
                gap: 10px;

                @include mobile {
                    // flex-direction: column;
                    flex-wrap: wrap;
                }
                .mess {
                    height: 100%;
                    max-width: 250px;
                    .logo {
                        font-family: 'Integral CF', sans-serif;
                        font-size: 32px;
                        letter-spacing: -0.09em;
                        font-weight: 800;
                        line-height: 38.4px;
                        text-align: left;
                        margin-bottom: 13px;
                    }
                    @include mobile {
                        height: fit-content;
                        width: 100%;
                        max-width: 1000px;
                    }
                }
                .menu {
                    @include mobile {
                        margin-top: 20px;
                    }
                }
                .about-title {
                    font-family: 'Satoshi';
                    font-size: 16px;
                    font-weight: 600;
                    line-height: 18px;
                    letter-spacing: 0px;
                    text-align: left;
                    margin-bottom: 15px;
                }
                .common-text {
                    width: 100%;
                    // height: 80%;
                    font-family: 'Satoshi';
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 27px;
                    text-align: left;
                    opacity: 60%;
                    /* margin-bottom: 40px; */
                }
            }
            .line-separation {
                margin: 0 auto;
                margin-top: 40px;
                max-width: 1440px;
                height: 2px;
                background-color: #0000001a;
                position: relative; /* Đảm bảo rằng nó cũng có position được định rõ */
            }
            .list-pay {
                max-width: 1440px;
                margin: 0 auto;
                height: 100px;
                display: flex;
                justify-content: space-between;
                align-items: center;
                @include mobile {
                    margin-top: 20px;
                    flex-wrap: wrap;
                    justify-content: center;
                    align-items: center;
                }
            }
        }
    }
}
</style>
