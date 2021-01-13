<template lang="html">
    <li v-on:click="handleClick">{{country.name}}</li>
</template>

<script>
export default {
    name: 'list-item',
    props: ['country'],
    methods: {
        handleClick: function() {
            console.log('country', this.country)
        }
    }

};
</script>

<style lang="css" scoped>


</style>