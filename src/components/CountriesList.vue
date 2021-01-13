<template lang="html">
    <div>
        <ul>
            <list-item v-for="(country, index) in countries" :country="country" :key="index"></list-item>
        </ul>
    </div>

  
</template>

<script>
import ListItem from './ListItem.vue';

export default {
    name: 'countries-list',
    props: ['countries'],
    components: {
        "list-item": ListItem
    }
};
</script>

<style lang="css" scoped>

ul {
        list-style-type: none;
        background-color: rgb(188, 190, 190);        
        padding: 5px 0px 0px 5px;
        margin-left: 0;
        height: 400px;
        width: 100%;
        overflow: hidden;
        overflow-y: scroll;
    }

</style>