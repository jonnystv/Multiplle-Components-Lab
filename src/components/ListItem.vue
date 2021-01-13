<template lang="html">
    <li v-on:click="handleClick">{{country.name}}</li>
</template>

<script>
import { eventBus } from '../main.js'

export default {
    name: 'list-item',
    props: ['country'],
    methods: {
        handleClick: function() {
            eventBus.$emit('country-selected', this.country);
        }
    }

}
</script>

<style lang="css" scoped>

    li {
        color: rgb(230, 230, 230);
        text-transform: uppercase;
        padding: 7px 5px 7px 5px;
        margin: 0px 5px 5px 5px;
        background-color: rgb(66, 66, 66);
        margin-left: 0;
        cursor: grab;
    }

    li:hover {
        background-color: rgb(230, 230, 230);
        color: rgb(66, 66, 66);
    }

</style>