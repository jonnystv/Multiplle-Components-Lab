<template lang="html">

    <div v-if='country'>
        <div class="main">
        <h3>{{ country.name }}</h3>
        <p><span>Capital:</span> {{ country.capital }}</p>
        <p><span>Pop.:</span> {{ country.population }}</p>
        <p><span>Area:</span> {{ country.area }} km<sup>2</sup></p>
        </div>
    </div>
  
</template>

<script>
export default {
    name: "country-detail",
    props: ['country']
};
</script>

<style lang="css" scoped>

    .main {
        width: 250px;
        margin-top: 15px;
        padding: 10px 20px 10px 20px;
        background-color: rgb(230, 230, 230);
        border: 5px solid rgb(66, 66, 66);
    }

    h3 {
        text-transform: uppercase;
        color: seagreen;
    }

    span {
        font-weight: bold;
    }

</style>