<script>
import Logo from '../lib/IMG/logo_header.png';
import Modal from './modal.svelte';
import Menu from './menu.svelte';
let escojerModal = false;

const abrirModal = () => {
    escojerModal = true;
}
const cerrarModal = () =>{
    escojerModal = false;
}
</script>
<div class="contenedor">
    <div class="logo">
        <a href="/"><img src={Logo} alt=""></a>  
       
    </div>
    <div class="login">
        <button type="button" class="fa-solid fa-user" on:click={abrirModal}> </button> 
    </div>
    <Menu />
    <div class="menu"></div>
</div>
<Modal abierto={escojerModal}  cerrar={cerrarModal}>
    <a href="">Olvido la contarseña</a>
</Modal>  

<style>
    .contenedor
    {
        position: relative;
        height: 300px;
        background: linear-gradient(-45deg,#628C88,#CDE8E8,#CDE8E8);
        display: flex;
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
        color: #CDE8E8;
        font-size: 70px;
        right: 4%;
        top: 6%;
        border: transparent;
        margin:5px;
        padding: 12px;
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
    @media (max-width: 850px)
    {
        .contenedor
        {
            height: 250px;
        }
    }
    
</style>