<template>
    <div class="container">
        <div class="title">
            OUR HAPPY CUSTOMERS
            <span class="material-symbols-outlined arrow-back">
                arrow_back
            </span>
            <span class="material-symbols-outlined arrow-forward">
                arrow_forward
            </span>
        </div>
        <div class="feetback-container">
            <BaseFeetback :username="username1" :feetback="feetback1" />
            <BaseFeetback :username="username2" :feetback="feetback2" />
            <BaseFeetback :username="username3" :feetback="feetback3" />
        </div>
    </div>
</template>
<script>
import BaseFeetback from '../UI/BaseFeetback.vue';
export default {
    data() {
        return {
            username1: 'Sarah M.',
            feetback1: `"I'm blown away by the quality and style of the clothes I received from Shop.co. From casual wear to elegant dresses, every piece I've bought has exceeded my expectations.”`,
            username2: 'Alex K.',
            feetback2: `"Finding clothes that align with my personal style used to be a challenge until I discovered Shop.co. The range of options they offer is truly remarkable, catering to a variety of tastes and occasions.”`,
            username3: 'James L.',
            feetback3: `"As someone who's always on the lookout for unique fashion pieces, I'm thrilled to have stumbled upon Shop.co. The selection of clothes is not only diverse but also on-point with the latest trends.”`,
        };
    },
    components: { BaseFeetback },
};
</script>
<style scoped>
.container {
    display: grid;
    justify-items: center;
    padding: 0px 100px;
    margin: 70px 0px;
}
.title {
    margin: 30px 0px;
    font-family: 'Integral CF', sans-serif;
    letter-spacing: -0.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
    margin-right: auto;
}
.arrow-back {
    position: absolute;
    right: 50px;
    cursor: pointer;
    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
    margin-right: 100px;
    justify-items: right;
    font-size: 40px;
}
.arrow-forward {
    position: absolute;
    right: 0;
    cursor: pointer;
    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
    margin-right: 100px;
    justify-items: right;
    font-size: 40px;
}
.feetback-container {
    display: flex;
    overflow-x: auto;
    max-width: 100%;
    gap: 20px;
}
@media (max-width: 768px) {
    .container {
        padding: 0px 25px;
        margin: 30px 0px;
    }
    .title {
        margin: 30px 0px;
        font-size: 40px;
        line-height: 40px;
        font-weight: 800;
        text-align: left;
        margin-right: auto;
    }
    .arrow-back {
        right: -40px;
        margin-right: 100px;
        font-size: 40px;
    }
    .arrow-forward {
        right: -80px;
        margin-right: 100px;
        font-size: 40px;
    }
}
</style>
