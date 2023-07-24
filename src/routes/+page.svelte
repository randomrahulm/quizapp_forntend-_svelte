<script lang='ts'>
    import quizz from "../data.json"
</script>



<div class="quiz_container w-[700px] h-screen m-auto flex justify-center items-center space-x-4"
>
    {#each quizz as quiz}
        <div class="quiz_card w-[250px] shadow overflow-hidden cursor-pointer ">
            <img class="h-44" src={quiz.imageUrl} alt="" >
            <div class="flex item-center justify-between py-3 px-2">
                <h1 class="font-bold">{quiz.name}</h1>
                <p>{``}</p>
            </div>
        </div>
    {/each}
    

</div>