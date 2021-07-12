<template>
    <div id="background">
        <h1>Trade or View your Stock Portfolio!</h1>
        <h3>You may Save & Load your Data...</h3>
        <h3>Click on "End Day" to begin a New Day!</h3>
        <hr>
        <h4>Your Current Funds: {{funds | currency }}</h4>
    </div>
</template>

<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds;
        }
    }
}
</script>

