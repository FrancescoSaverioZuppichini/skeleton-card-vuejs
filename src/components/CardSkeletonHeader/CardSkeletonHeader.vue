<template>
<v-card-text>
    <v-layout row align-center>
        <v-flex>
            <div class='skeleton-card__header__avatar'>
            </div>
        </v-flex>
        <v-flex class="flex--grow">
            <v-layout column>
                <div class="skeleton-card__header__title grey">
                </div>
                <div class="skeleton-card__header__subtitle grey lighten-1 mt-1">
                </div>
            </v-layout>
        </v-flex>
    </v-layout>
</v-card-text>
</template>

<script>
export default {
    name: "",
    components: {

    },
    data: function() {
        return {}
    },
    methods: {}
}
</script>

<style scoped>
.skeleton-card__header__avatar {
    border-radius: 50%;
    height: 50px;
    width: 50px;
    background-color: grey;
}

.skeleton-card__header__subtitle {
    width: 70%;
    height: 12px;
}

.skeleton-card__header__title {
    width: 100%;
    height: 14px;
}
</style>