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
    /* opacity: 60%; */
}
.view-all:hover {
    background-color: #eeeeee;
}
</style>
