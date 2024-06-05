<template>
    <div>
        <div
            class="item-image"
            :style="{ backgroundImage: 'url(' + dynamicImage + ')' }"
        ></div>
        <div class="item-name">{{ itemName }}</div>
        <div class="item-rate">
            <svg
                width="150"
                height="19"
                viewBox="0 0 150 19"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
            >
                <path
                    d="M9.24494 0.255066L11.8641 5.89498L18.0374 6.64316L13.4829 10.877L14.679 16.9793L9.24494 13.9561L3.8109 16.9793L5.00697 10.877L0.452479 6.64316L6.62573 5.89498L9.24494 0.255066Z"
                    fill="#FFC633"
                />
                <path
                    d="M33.0469 0.25502L35.6661 5.89493L41.8394 6.64312L37.2849 10.877L38.481 16.9793L33.0469 13.956L27.6129 16.9793L28.809 10.877L24.2545 6.64312L30.4277 5.89493L33.0469 0.25502Z"
                    fill="#FFC633"
                />
                <path
                    d="M56.8487 0.25502L59.4679 5.89493L65.6412 6.64312L61.0867 10.877L62.2827 16.9793L56.8487 13.956L51.4147 16.9793L52.6107 10.877L48.0562 6.64312L54.2295 5.89493L56.8487 0.25502Z"
                    fill="#FFC633"
                />
                <path
                    d="M80.6507 0.25502L83.2699 5.89493L89.4432 6.64312L84.8887 10.877L86.0847 16.9793L80.6507 13.956L75.2167 16.9793L76.4127 10.877L71.8582 6.64312L78.0315 5.89493L80.6507 0.25502Z"
                    fill="#FFC633"
                />
                <path
                    d="M98.5659 16.9793L104 13.956V0.25502L101.381 5.89493L95.2075 6.64311L99.762 10.877L98.5659 16.9793Z"
                    fill="#FFC633"
                />
                <path
                    d="M124.98 12.872H123.804V15H122.824V12.872H117.56V11.976L122.46 4.976H123.804V11.976H124.98V12.872ZM118.652 11.976H122.824V6.012L118.652 11.976ZM127.242 15.154C126.766 15.154 126.36 14.762 126.36 14.3C126.36 13.824 126.766 13.418 127.242 13.418C127.718 13.418 128.124 13.824 128.124 14.3C128.124 14.762 127.718 15.154 127.242 15.154ZM132.763 15.168C130.747 15.168 129.459 13.908 129.459 11.934H130.467C130.467 13.376 131.349 14.244 132.777 14.244C134.289 14.244 135.269 13.236 135.269 11.752C135.269 10.352 134.359 9.246 132.777 9.246C131.853 9.246 131.013 9.666 130.467 10.268L129.669 10.016L130.873 4.976H135.717V5.9H131.601L130.845 9.05C131.405 8.602 132.133 8.35 132.917 8.35C135.003 8.35 136.291 9.848 136.291 11.724C136.291 13.74 134.863 15.168 132.763 15.168ZM137.817 15H136.865L140.771 4.976H141.751L137.817 15Z"
                    fill="black"
                />
                <path
                    d="M145.806 15.168C143.79 15.168 142.502 13.908 142.502 11.934H143.51C143.51 13.376 144.392 14.244 145.82 14.244C147.332 14.244 148.312 13.236 148.312 11.752C148.312 10.352 147.402 9.246 145.82 9.246C144.896 9.246 144.056 9.666 143.51 10.268L142.712 10.016L143.916 4.976H148.76V5.9H144.644L143.888 9.05C144.448 8.602 145.176 8.35 145.96 8.35C148.046 8.35 149.334 9.848 149.334 11.724C149.334 13.74 147.906 15.168 145.806 15.168Z"
                    fill="black"
                    fill-opacity="0.6"
                />
            </svg>
            <v-rating
                v-model="rating"
                active-color="yellow-darken-2"
                :half-increments="true"
                color="white"
                :length="5"
                density="compact"
                readonly
            ></v-rating>
        </div>
        <div class="item-price">{{ itemPrice }}</div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            rating: 3,
        };
    },
    props: ['buttonName', 'dynamicImage', 'itemName', 'itemPrice'],
};
</script>
<style scoped>
.item-image {
    width: 295px;
    height: 298px;
    background-size: cover;
    border-radius: 15px;
    display: block;
    align-items: center;
    background-position: center;
}
.item-name {
    margin-top: 10px;
    font-family: 'Satoshi', sans-serif;
    font-size: 15px;
    font-weight: 700;
    line-height: 27px;
    text-align: left;
}
.item-rate {
    margin-top: 5px;
}
.item-price {
    font-family: 'Satoshi', sans-serif;
    margin-top: 5px;
    font-size: 24px;
    font-weight: 700;
    line-height: 32.4px;
    text-align: left;
}
@media (max-width: 768px) {
    .item-image {
        width: 235px;
        height: 238px;
    }
}
</style>
