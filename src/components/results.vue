<script>
    export default {
        name: "resultsSecion"
    }
</script>

<template>

    <section class="results-section">
        <h2>Your Result</h2>
        <div class="result-value">
            <p>76</p>
        </div>
        <p class="avaliation">Great</p>
        <p class="avaliation-description">
            you score higher then 65% of the people who have taken these tests.
        </p>
    </section>

</template>

<style scoped>
    .results-section {
        width: 50%;
        height: 100%;
        background: linear-gradient(to top, hsl(241, 81%, 54%) 0%, hsl(252, 100%, 67%) 100%); 
        border-radius: 2em;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 60px;
    }
    .results-section h2 {
        color: hsl(241, 100%, 89%);
    }
    .results-section .result-value {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        background: linear-gradient(to bottom   , rgba(0, 0, 0, 0.243) 0%, rgba(78, 33, 202, 0.1) 100%);  
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 30px 0; 
    }
    .results-section .result-value p {
        font-size: 4em;
        font-weight: 800;
        position: relative;
    }
    .results-section .result-value p::after {
        content: "of 100";
        position: absolute;
        font-size: 16px;
        font-weight: 500;
        color: hsl(241, 100%, 89%);
        top: 90%;
        left: 13px;
        width: 100px;
    }
    .results-section .avaliation {
        font-size: 1.5em;
        font-weight: 700;
    }
    .results-section .avaliation-description {
        margin-top: 10px;
        text-align: center;
        font-weight: 500;
        color: hsl(241, 100%, 89%);
    }

    @media (max-width: 760px){
        .results-section {
            width: 100vw;
            border-radius: 0 0 2em 2em;
        }
    }
</style>
