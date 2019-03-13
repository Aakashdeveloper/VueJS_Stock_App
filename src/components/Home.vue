<template>
    <div class="text_home">
        <h1>Trade or View your Portfolio</h1>
        <h4>You may Save & Load your Data</h4>
        <h6 >Click on 'End Day' to begin a New Day!</h6>
        <hr>
        <p >Your Funds: {{ funds | currency }}</p>
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