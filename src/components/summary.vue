<script>
    import reaction from "./reaction.vue"
    import memory from "./memory.vue" 
    import verbal from "./verbal.vue"
    import visual from "./visual.vue"
    export default {
        name: "summarySection",
        components: {
            reaction,
            memory,
            verbal,
            visual
        }
    }
</script>

<template>
    <section class="summary-section">
        <h2>Summary</h2>
        <div class="rate">
            <reaction/>
            <memory/>
            <verbal/>
            <visual/>
        </div>
        <button>Continue</button>
    </section>
</template>

<style scoped>
    .summary-section {
        padding: 40px;
    }
    .summary-section h2 {
        color: hsl(224, 30%, 27%);
    }
    .summary-section .rate {
        margin: 40px 0;
    }
    .summary-section button {
        width: 290px;
        height: 56px;
        border-radius: 2em;
        color: hsl(221, 100%, 96%);
        background-color: hsl(224, 30%, 27%);
        transition: .2s;
    }
    .summary-section button:hover {
        background:linear-gradient(to top, hsl(241, 81%, 54%) 0%, hsl(252, 100%, 67%) 100%);
    }

    @media (max-width: 760px) {
      .summary-section {
            width: 100vw;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
    }
</style>