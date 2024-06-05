<template>
    <div class="feedback-container">
        <div class="wrapper">
            <div class="title">
                OUR HAPPY CUSTOMERS
                <div class="actions-feedback">
                    <span class="material-symbols-outlined arrow-back">
                        arrow_back
                    </span>
                    <span class="material-symbols-outlined arrow-forward">
                        arrow_forward
                    </span>
                </div>
            </div>
            <div class="feetback-group">
                <BaseFeetback :username="username1" :feetback="feetback1" />
                <BaseFeetback :username="username2" :feetback="feetback2" />
                <BaseFeetback :username="username3" :feetback="feetback3" />
            </div>
        </div>
    </div>
</template>
<script>
import BaseFeetback from '../../ui/body/item/BaseFeedback.vue';
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
<style lang="scss" scoped>
@import '../../../assets/styles/global.scss';
.feedback-container {
    padding: 0 100px;
    margin-bottom: 50px;
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
        width: 100%;
        margin: 0 auto;
        max-width: 1440px;
        .title {
            margin: 30px 0px;
            font-family: 'Integral CF', sans-serif;
            letter-spacing: -0.07em;
            font-size: 48px;
            font-weight: 800;
            line-height: 57.6px;
            display: flex;
            // text-align: center;

            .actions-feedback {
                margin-left: auto;
                .material-symbols-outlined {
                    cursor: pointer;
                    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0,
                        'opsz' 24;
                    font-size: 40px;
                    @include mobile {
                        display: none;
                    }
                    margin: 0px 4px;
                }
            }
        }
        .feetback-group {
            display: flex;
            overflow-x: auto;
            max-width: 100%;
            gap: 20px;
        }
    }
}
</style>
