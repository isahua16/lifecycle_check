<template>
    <div>
        <h1>Hello!</h1>
    </div>
</template>

<script>
    export default {
        beforeCreate: function()
        {
            console.log(`I am in beforeCreate cycle`);
        },
        created: function()
        {
            console.log(`I am in created cycle`);
        },
        beforeMount: function()
        {
            console.log(`I am in beforeMount cycle`);
        },
        mounted: function()
        {
            console.log(`I am in mounted cycle`);
        },
    }
</script>

<style scoped>

</style>