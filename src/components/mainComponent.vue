<script>
    import resultsSection from "./results.vue";
    import summarySection from "./summary.vue";
    export default {
        name: "mainComponent",
        components: {
            resultsSection,
            summarySection
        }
    }
</script>

<template>
    <main>
        <resultsSection/>
        <summarySection/>
    </main>
</template>

<style scoped>
    main {
        width: 750px;
        height: 510px;
        border-radius: 2em;
        box-shadow: 0px 3px 14px 0px hsla(224, 30%, 27%, 0.291);
        display: flex;
    }

    @media (max-width:760px) {
        main {
            width: 100vw;
            height: auto;
            flex-direction: column;
        }
    }
</style>
