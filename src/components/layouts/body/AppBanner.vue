<template>
    <div class="intro-container">
        <div class="wrapper">
            <div class="left-intro">
                <div class="first-content">
                    FIND CLOTHES THAT MATCHES YOUR STYLE
                </div>
                <div class="second-content">
                    Browse through our diverse range of meticulously crafted
                    garments, designed to bring out your individuality and cater
                    to your sense of style.
                </div>
                <button class="shop-now">Shop Now</button>
                <div class="detail-infor">
                    <div class="amount-cont">
                        <div class="amount">200+</div>
                        <div class="type-amount">International Brands</div>
                    </div>
                    <div class="amount-cont">
                        <div class="amount">2,000+</div>
                        <div class="type-amount">High-Quality Products</div>
                    </div>
                    <div class="amount-cont">
                        <div class="amount">30,000+</div>
                        <div class="type-amount">Happy Customers</div>
                    </div>
                </div>
            </div>
            <div class="right-intro">
                <div class="image-banner"></div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../../../assets/styles/global.scss';
.intro-container {
    background-color: #f2f0f1;
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
        height: 100%;
        display: flex;
        max-width: 1440px;
        margin: 0px auto;

        @include tablet {
            height: fit-content;
            flex-direction: column;
            width: 100%;
        }
        @include mobile {
            flex-direction: column;
            width: 100%;
        }
        .left-intro {
            width: 50%;
            margin: 100px 0px;
            background-color: #f2f0f1;
            align-content: center;

            @include tablet {
                display: flex;
                justify-content: center;
                width: 100%;
                height: 250px;
                flex-direction: column;
                justify-items: center;
            }
            @include mobile {
                margin: 50px 0px;
                align-content: center;
                width: 100%;
                height: fit-content;
            }
            .first-content {
                max-width: 577px;
                font-family: 'Integral CF', sans-serif;
                letter-spacing: -0.05em;
                font-size: 64px;
                font-weight: 900;
                line-height: 60px;
                text-align: left;
                margin-bottom: 32px;
                @include medium-screen {
                    font-size: 56px;
                    font-weight: 800;
                    line-height: 50px;
                    text-align: left;
                }
                @include tablet {
                    max-width: 800px;
                    width: 100%;
                    font-size: 56px;
                    font-weight: 800;
                    line-height: 50px;
                    text-align: center;
                    margin-left: auto;
                    margin-right: auto;
                }
                @include mobile {
                    max-width: 577px;
                    font-size: 41px;
                    text-align: center;
                    font-weight: 800;
                    line-height: 40px;
                }
            }
            .second-content {
                max-width: 545px;
                font-family: 'Satoshi';
                font-size: 16px;
                font-weight: 400;
                line-height: 22px;
                text-align: left;
                opacity: 60%;
                margin-bottom: 32px;
                @include medium-screen {
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 22px;
                    text-align: left;
                }
                @include tablet {
                    max-width: 600px;
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 22px;
                    margin-bottom: 0px;
                    text-align: center;
                    margin-left: auto;
                    margin-right: auto;
                }
                @include mobile {
                    max-width: 520px;
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 22px;
                }
            }
            .shop-now {
                padding: 14px 65px 14px 65px;
                border-radius: 30px;
                background: black;
                color: white;
                margin-bottom: 40px;
                @include tablet {
                    // margin-bottom: 20px;
                    max-width: 465px;
                    margin: 32px auto;
                    width: 100%;
                }
                @include mobile {
                    // margin-bottom: 20px;
                    max-width: 465px;
                    margin: 32px auto;
                    width: 100%;
                }

                cursor: pointer;
            }
            .shop-now:hover {
                background-color: #000000c2;
            }
            .detail-infor {
                display: flex;
                gap: 45px;
                @include medium-screen {
                    gap: 20px;
                }
                @include tablet {
                    flex-wrap: wrap;
                    justify-content: center;
                }
                @include mobile {
                    gap: 20px;
                }
            }
            .amount-cont {
                box-sizing: border-box;
                text-align: center;
                .amount {
                    font-family: 'Satoshi';
                    font-size: 40px;
                    font-weight: 700;
                    line-height: 54px;
                    text-align: left;

                    @include tablet {
                        font-size: 30px;
                        font-weight: 800;
                        line-height: 40px;
                        display: contents;
                    }
                    @include mobile {
                        gap: 20px;
                    }
                }
                .type-amount {
                    font-family: 'Satoshi';
                    font-size: 16px;
                    font-weight: 400;
                    line-height: 22px;
                    text-align: left;
                    white-space: nowrap;
                    opacity: 60%;
                }
            }
        }
        .right-intro {
            align-content: center;
            width: 50%;
            height: 100%;
            @include tablet {
                height: 500px;
                width: 100%;
                padding: 0 100px;
            }
            @include mobile {
                width: 100%;
                height: 440px;
                padding: 0 20px;
            }
            .image-banner {
                width: 100%;
                height: 100%;
                background: url('../../../assets/images/background-intro.jpg')
                    center center no-repeat;
                background-size: cover;
                transform-origin: top;
                /* background-position: top; */
                background-position-y: -59px;
                @include mobile {
                    background-position-y: -47px;
                }
            }
        }
    }
}
</style>
