<template lang="html">

    <div v-if='country'>
        <p>
        <h3>{{ country.name }}</h3>
        <p>{{ country.capital }}</p>
        <p>{{ country.population }}</p>
        <p>{{ country.area }}</span></p>
        </p>
    </div>
  
</template>

<script>
export default {
    name: "country-detail",
    props: ['country']
};
</script>

<style lang="css" scoped>
</style>