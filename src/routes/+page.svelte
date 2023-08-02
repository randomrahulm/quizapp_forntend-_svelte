<script lang='ts'>
    import quizz from "../data.json"

    import Cards from "../components/Card.svelte"

    
</script>




{#each quizz as quiz}
    <Cards {quiz} />
{/each}
    

