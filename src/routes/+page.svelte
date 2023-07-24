<script lang='ts'>
    import quizz from "../data.json"

    import Cards from "../components/Card.svelte"

    
</script>



<div class="quiz_container w-[700px] h-screen m-auto flex justify-center items-center space-x-4"
>
    {#each quizz as quiz}
        <Cards {quiz} />
    {/each}
    

</div>