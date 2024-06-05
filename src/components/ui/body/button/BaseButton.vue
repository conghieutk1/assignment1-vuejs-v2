<template>
    <button class="view-all">{{ buttonName }}</button>
</template>
<script>
export default {
    props: ['buttonName'],
};
</script>
<style scoped>
.view-all {
    width: 218px;
    height: 52px;
    padding: 16px 54px 16px 54px;
    gap: 12px;
    border-radius: 62px;
    border: 1px solid #0000001a;
    background-color: white;
    cursor: pointer;
    display: flex;
    margin: 0px auto;
    justify-content: center;
    align-items: center;
    /* opacity: 60%; */
}
.view-all:hover {
    opacity: 80%;
    color: #000;
    border: 1px solid black;
}
</style>
