<template>
    <div class="text-center">
        <v-rating
            class="star"
            v-model="rating"
            half-increments
            hover
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
