<script>
    export let showabout=false;
</script>
<main>
    {#if showabout}
    <div class="backdrop" on:click>
        <div class="modal">
            <p>So this is subramaniyan srinivasan(also vishal)....</p>
            <p>I am a 1st yr student in SASTRA university and i am learning web development</p>
            <p>My github and linkedin profile is given below :) , make sure to check it out</p>
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
