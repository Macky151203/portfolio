<script>
    export let showmodal=false;
</script>
<main>
    {#if showmodal}
    <div class="backdrop" on:click>
        <div class="modal">
            <p>you are in homepage only, dont click it again.....</p>
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