<template>
<v-card-title primary-title>
    <div class="skeleton-card__title grey darken-2 mb-1">
    </div>
    <div :key="line" v-for="line in lines" class='skeleton-card__text mt-1 grey lighten-1'>
    </div>
</v-card-title>
</template>

<script>
export default {
    name: "",
    props: {
        'lines': {
            default: 2
        }
    }
}
</script>

<style scoped>

.skeleton-card__title {
    width: 100%;
    height: 24px;
}

.skeleton-card__text {
    width: 100%;
    height: 16px;
}
</style>