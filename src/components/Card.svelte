<script lang='ts'>
    import { goto } from "$app/navigation"
    
    interface Quiz {
        id:number;
        name:string;
        imageUrl:string;
        questions:{
            id:number;
            question:string;
            options:{
                id:number;
                text:string;
                label:string;
            }[];
            answers:string;
        }[];
    }
    
    export let quiz:Quiz;
</script>


<button on:click={goto(`/quiz/${quiz.id}`)}>
<div class="quiz_card w-[250px] shadow overflow-hidden cursor-pointer ">
    <img class="h-44" src={quiz.imageUrl} alt="" >
    <div class="flex item-center justify-between py-3 px-2">
        <h1 class="font-bold">{quiz.name}</h1>
        <p>{quiz.questions.length} questions</p>
    </div>
</div>
</button>