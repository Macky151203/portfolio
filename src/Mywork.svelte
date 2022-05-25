<script>
    export let showwork=false;
</script>
<main>
    {#if showwork}
    <div class="backdrop" on:click>
        <div class="modal">
            <p>I havent made lots of projects so far.... made a todo list and this website and the link for the todo list is given below. And also my blog link is given below as well</p>
            <a href="https://manageday.vercel.app/" target="_blank">Todo list</a>
            <a href="https://subro.hashnode.dev/first-blog" target="_blank">My blog</a>
        </div>
    </div>
    {/if}
</main>
<style>
    .backdrop{
        width: 100%;
        height: 100%;
        position: fixed;
        background-color: rgba(0, 0, 0, 0.47);


    }
    .modal{ 
        padding: 15px;
        border-radius: 20px;
        max-width: 500px;
        margin: 10% auto;
        text-align: center;
        background: white;
        box-shadow: 2px 3px 2px 3px rgb(229, 223, 223);
        z-index: 2;
    }
    p{
        font-family: fantasy;
    }
    @media screen and (max-width:540px){
        .modal{
            margin: 20px;
        }
    }
</style>
