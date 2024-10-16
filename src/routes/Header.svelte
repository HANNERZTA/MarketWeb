<script>
import Logo from '../lib/IMG/logo_header.png';
import Modal from './modal.svelte';

let escojerModal = false;

const abrirModal = () => {
    escojerModal = true;
}
const cerrarModal = () =>{
    escojerModal = false;
}
</script>
<header class="contenedor">
    <div class="logo">
        <a href="/"><img src={Logo} alt=""></a>  
       
    </div>
    <button type="button" class="fa-solid fa-user" on:click={abrirModal}> </button> 

      
    <div class="boton">
        <button><a href="/quesomos">Quienes somos</a></button>
        <button><a href="/planes">Planes</a></button>
        <button><a href="/mision">Misión y Visón</a></button>
    </div>
    <div class="menu">
    
    </div>
</header>
<Modal abierto={escojerModal}  cerrar={cerrarModal}>
    <a href="">Olvido la contarseña</a>
</Modal>  
<style>
    .contenedor
    {
        position: relative;
        width: 100%;
        height: 50vh;
        background: linear-gradient(-45deg,#628C88,#CDE8E8,#CDE8E8);
        overflow: hidden;

    }
    .menu
    {
       position: absolute;
       bottom: 0;
       left: 0;
       width: 100%;
       height: 100px;
       background-image: url(../lib/IMG/ola.png);
       background-size: 1000px 100px;
       animation: menu 20s linear infinite;
    }
    .logo
    {
        position: absolute;
        top:10%;
        left: 5%;
    }
    .fa-solid
    {
        position: absolute;
        color: #628C88;
        font-size: 50px;
        right: 4%;
        top: 5%;
        border: transparent;
        margin:5px;
        padding: 12px;
    }
    .boton
    {
        position: absolute;
        bottom: 30%;
        left: 20rem;
        
    }
    button
    {
        margin: 50px;
        padding: 10px;
        font-size: 15px;
        background: transparent;
        border-radius:50px;
        border: solid 0.5px transparent;
        color: #628C88;
    }
    a
    {
        text-decoration: none;
        color: #628C88;
    }
    button:hover
    {
        padding-left: 12px;
        color: white;
        border: solid 0.5px white;
    }
    @keyframes menu
    {
        0%{
            background-position-x: 0;
        }
        100%{
            background-position-x: 1000px;
        }
    }
    
</style>