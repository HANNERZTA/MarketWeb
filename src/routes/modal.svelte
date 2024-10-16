<script>
    import Logo from "../lib/IMG/MarketWeb_login.png";
    export let abierto = false;
    export let cerrar;

    const cerrarModal = () => {
        cerrar();
    };
</script>

{#if abierto}
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <div class="modal-overlay" on:click={cerrarModal}>
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-static-element-interactions -->
        <div class="moda" on:click|stopPropagation>
            <div class="logo">
                <img src={Logo} alt="" />
            </div>
            <div class="inputs">
                <input type="text" placeholder="Usuario" />
                <input type="password" placeholder="********" />
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
        background: #cde8e8;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        color: #628c88;
        display: grid;
    }
    input {
        color: #628c88;
        display: flow-root;
        margin: 10px;
        margin-bottom: 0px;
        width: 300px;
        border-radius: 10px;
        border: 1px solid white;
        padding: 2px;
        background: #cde8e8;
    }
    .logo {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    button {
        border-radius: 10px;
        padding: 5px;
        border: 1px solid transparent;
        background: #628c88;
        color: white;
        margin: 10px;
    }
</style>
