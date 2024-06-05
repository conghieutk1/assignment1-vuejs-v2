<template>
    <div class="text-center">
        <v-rating
            v-model="ratingNumber"
            active-color="yellow-darken-2"
            :half-increments="true"
            color="red"
            :length="5"
            density="compact"
            readonly
        ></v-rating>
    </div>
</template>

<script>
export default {
    data() {
        return {
            ratingNumber: 3,
        };
    },
    // props: ['ratingNumber'],
};
</script>
<style scoped>
.text-center {
    position: relative;
    z-index: 1000;
}
</style>
