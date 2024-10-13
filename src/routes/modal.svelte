<script>
    import Logo from '../lib/IMG/Logo.png'
    export let abierto= false;
    export let titulo= '';
    export let cerrar;

    const cerrarModal = () =>{
        cerrar();
    }
</script>
{#if abierto}
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <div class="modal-overlay" on:click={cerrarModal}>
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-static-element-interactions -->
        <div class="moda" on:click|stopPropagation>
            <img src={Logo} alt="" class="logo">
            <button class="registro">Registro</button>
            <h2>{titulo}</h2>  
            <div class="inputs">
                <input type="text" placeholder="Usuario">
                <input type="password" placeholder="********">
            </div>
            <slot></slot>
            <button on:click={cerrarModal} class="entrar">Aceptar</button>
        </div>
    </div>
{/if}
<style>
    .modal-overlay {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(0, 0, 0, 0.7);
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .moda {
        background: #CDE8E8;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        color: #628C88;
        position: relative;
        display: grid;
    }
    input
    {
        color: #628C88;
        display: flow-root;
        margin: 10px;
        margin-bottom: 0px;
        width: 300px;
        border-radius:10px;
        border: 1px solid white;
        padding: 2px;
        background: #CDE8E8;
    
    }
    .registro
    {
        position: absolute;
        top: 5%;
        right: 5%;
    }
    .logo
    {
        justify-content: center;
    } 
    button
    {
        border-radius: 10px;
        padding: 5px;
        border: 1px solid transparent;
        background: #628C88;
        color: white;
        margin: 10px;
    }   
</style>