<template>
<v-card>
    <card-skeleton-header v-if="hasHeader">
    </card-skeleton-header>
    <v-container v-if="isHorizontal">
        <v-layout row align-center>
            <v-flex class="flex--grow">
                <card-skeleton-text :lines="lines">
                </card-skeleton-text>
            </v-flex>
            <v-flex>
                <card-skeleton-media height="150px" width="150px" v-if="hasMedia">
                </card-skeleton-media>
            </v-flex>
        </v-layout>
    </v-container>
    <v-layout column v-else>
        <v-flex>
            <card-skeleton-media v-if="hasMedia">
            </card-skeleton-media>
        </v-flex>
        <v-flex>
            <card-skeleton-text :lines="lines" v-if="hasText">
            </card-skeleton-text>
        </v-flex>
    </v-layout>
    <card-skeleton-actions v-if="hasActions">
    </card-skeleton-actions>
</v-card>
</template>

<script>
import CardSkeletonHeader from './CardSkeletonHeader/CardSkeletonHeader.vue'
import CardSkeletonMedia from './CardSkeletonMedia/CardSkeletonMedia.vue'
import CardSkeletonText from './CardSkeletonText/CardSkeletonText.vue'
import CardSkeletonActions from './CardSkeletonActions/CardSkeletonActions.vue'

export default {
    name: "",
    props: {
        'hasHeader': {
            default: true
        },
        'hasMedia': {
            default: true
        },
        'hasText': {
            default: true
        },
        'hasActions': {
            default: false
        },
        'isHorizontal': {
            default: false
        },
        'lines': {
            default: 2
        }
    },
    components: {
        CardSkeletonHeader,
        CardSkeletonMedia,
        CardSkeletonText,
        CardSkeletonActions
    },
    data: function() {
        return {}
    },
    methods: {}
}
</script>

<style>
.flex--grow {
    flex-grow: 99 !important;
}
</style>