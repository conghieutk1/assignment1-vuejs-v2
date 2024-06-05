<template>
    <div class="text-center">
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
</template>
<script>
export default {
    data: () => ({
        rating: 3.5,
    }),
};
</script>
<style scoped>
.star {
    color: red !important;
}
</style>
