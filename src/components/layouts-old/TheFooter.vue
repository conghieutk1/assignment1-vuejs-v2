<template>
    <div class="footer-container">
        <div class="stay-uptodate">
            <div class="text-uptodate">
                STAY UPTO DATE ABOUT OUR LATEST OFFERS
            </div>
            <div class="get-infor">
                <div class="box-enter-email">
                    <span class="material-symbols-outlined"> mail </span>

                    <input
                        class="input-email"
                        placeholder="Enter your email address"
                    />
                </div>
                <button>Subscribe to Newsletter</button>
            </div>
        </div>
        <div class="contact-list">
            <div class="about-container">
                <div class="mess">
                    <div class="logo">SHOP.CO</div>
                    <p class="common-text">
                        We have clothes that suits your style and which you’re
                        proud to wear. From women to men.
                    </p>
                </div>
                <div class="company">
                    <div class="about-title">COMPANY</div>
                    <div class="common-text">About</div>
                    <div class="common-text">Features</div>
                    <div class="common-text">Works</div>
                    <div class="common-text">Carrer</div>
                </div>
                <div class="help">
                    <div class="about-title">HELP</div>
                    <div class="common-text">Customer Support</div>
                    <div class="common-text">Delivery Details</div>
                    <div class="common-text">Terms and Conditions</div>
                    <div class="common-text">Privacy policy</div>
                </div>
                <div class="faq">
                    <div class="about-title">F A Q</div>
                    <div class="common-text">Account</div>
                    <div class="common-text">Manage Deliveries</div>
                    <div class="common-text">Orders</div>
                    <div class="common-text">Payments</div>
                </div>
                <div class="resources">
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
</template>
<style scoped>
.footer-container {
    width: 100%;
    height: fit-content;
    /* background-color: #f0f0f0; */
    /* opacity: 10%; */
    background-color: white;
    position: relative;
}
.stay-uptodate {
    margin: 0px 100px;
    height: fit-content;
    border-radius: 20px;
    color: white;
    background-color: black;
    z-index: 2;
    position: relative;
    display: flex;
}
.text-uptodate {
    width: 50%;
    font-size: 40px;
    font-family: 'Integral CF', sans-serif;
    letter-spacing: -0.07em;
    font-weight: 800;
    line-height: 40px;
    text-align: left;
    align-content: center;
    /* margin-left: 50px; */
    padding: 0px 50px;
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
.material-symbols-outlined {
    color: #000;
    opacity: 60%;
    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
    justify-items: right;
}
.get-infor {
    width: 50%;
    display: flex;
    /* border: 1px solid red; */
    flex-direction: column;
    margin: 35px 50px;
    /* padding: 0px 30px 0px 250px; */
    gap: 10px;
    /* display: grid; */
}
.box-enter-email {
    height: 48px;
    border-radius: 30px;
    outline: none;
    display: flex;
    justify-items: center;
    align-items: center;
    background-color: #ffffff;
    /* padding-top: 12px; */
    gap: 10px;
    padding-left: 20px;
    width: 65%;
    margin-left: auto;
}
.input-email {
    height: 48px;
    width: 100%;
    border-radius: 30px;
    border: 1px solid transparent;
    outline: none;
    background-color: #ffffff;
}
button {
    height: 48px;
    border-radius: 30px;
    outline: none;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 500;
    line-height: 21.6px;
    text-align: center;
    background-color: #ffffff;
    cursor: pointer;
    width: 65%;
    margin-left: auto;
}
.contact-list {
    background-color: #f0f0f0;
    position: absolute;
    margin-top: -90px;
    width: 100%;
    height: fit-content;
    z-index: 1;
}
.about-container {
    height: 350px;
    width: 100%;
    padding: 150px 100px;
    display: flex;
    justify-content: space-between;
    gap: 10px;
}
.mess {
    width: 35%;
    height: 100%;
    padding-right: 130px;
}
.logo {
    font-family: 'Integral CF', sans-serif;
    font-size: 32px;
    letter-spacing: -0.09em;
    font-weight: 800;
    line-height: 38.4px;
    text-align: left;
    margin-right: 50px;
}
.common-text {
    width: 100%;
    height: 80%;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 27px;
    text-align: left;
    opacity: 60%;
    /* margin-bottom: 40px; */
}
.about-title {
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 600;
    line-height: 18px;
    letter-spacing: 3px;
    text-align: left;
    margin-bottom: 15px;
}
.company {
    width: 15%;
    height: 100%;
}
.help {
    width: 20%;
    height: 100%;
}
.faq {
    width: 15%;
    height: 100%;
}
.resources {
    width: 15%;
    height: 100%;
}
.line-separation {
    width: calc(100% - 200px); /* Thêm phần trừ đi margin ở hai bên */
    height: 1px;
    background-color: #000000;
    opacity: 0.3; /* Đặt opacity đúng */
    margin: 20px 100px 0px 100px;
    position: relative; /* Đảm bảo rằng nó cũng có position được định rõ */
}
.list-pay {
    width: calc(100% - 200px);
    height: 100px;
    margin: 0px 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

@media (max-width: 768px) {
    .stay-uptodate {
        margin: 0px 25px;
        padding: 30px 0px;
        display: flex;
        flex-direction: column;
        padding: ;
    }
    .text-uptodate {
        width: 100%;
        padding: auto;
        justify-content: center;
        margin-bottom: 30px;
        padding: 0px 20px;
        font-size: 40px;
        font-weight: 800;
        line-height: 35px;
        text-align: left;
    }
    .get-infor {
        width: 85%;
        display: flex;
        flex-direction: column;
        margin: 0px auto;
        gap: 10px;
    }
    .box-enter-email {
        width: 100%;
        /* margin-left: auto; */
    }
    button {
        width: 100%;
    }
    .contact-list {
        /* display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        width: 100%; */
        padding: 0;
    }
    .about-container {
        height: fit-content;
        width: 100%;
        padding: 150px 25px 0px 25px;
        display: flex;
        justify-content: space-between;
        gap: 10px;
        flex-wrap: wrap;
        /* flex-direction: column; */
        width: 100%;
    }
    .mess {
        width: 100%;
        padding-right: 0px;
    }
    .company {
        width: fit-content;
        height: 100%;
    }
    .help {
        width: fit-content;
        height: 100%;
    }
    .faq {
        width: fit-content;
        height: 100%;
    }
    .resources {
        width: fit-content;
        height: 100%;
    }
    .line-separation {
        width: calc(100% - 50px); /* Thêm phần trừ đi margin ở hai bên */
        margin: 20px auto;
    }
    .list-pay {
        width: calc(100% - 50px);
        height: 100px;
        margin: 0px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
    .list-pay-2 {
    }
}
</style>
