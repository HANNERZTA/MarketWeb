<script>
import Logo from '../lib/IMG/MarketWeb.png';
</script>
<header class="contenedor">
    <div class="logo">
        <img src={Logo} alt="">   
    </div>
    <i class="fa-solid fa-user"></i>
    <div class="boton">
        <button>Quenes somos</button>
        <button>Planes</button>
        <button>Misión y Visón</button>
    </div>
    <div class="menu">
    
    </div>
</header>
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
        right: 5%;
        top: 10%;
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
        border: solid 0.5px #628C88;
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