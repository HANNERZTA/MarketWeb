<script>
//     import { onMount } from 'svelte';
//     let scrolled= false;

// const handleScroll = () =>{
//     scrolled = window.scrollY > 50;
// };

// onMount(() =>{
//     window.addEventListener('scroll', handleScroll);
//     return () =>{
//         window.removeEventListener('scroll',handleScroll);
//     }
// });
</script>
<div class="boton">
    <!-- <nav class="menu" class:scrolled={scrolled}> -->
        <ul>
            <li><a href="/">Inicio</a></li>
            <li><a href="/Servicios">Servicios</a></li>
            <li><a href="/Nosotros">Sobre nosotros</a></li>
            <li><a href="/Contacto">Contacto</a></li>
        </ul>
    <!-- </nav> -->
</div>
<style>
    .boton
    {
            /* display: none; */
            position: absolute;
            top:20%;
            left: 50%;
            transform: translate(-50%, -50%);  
			z-index: 1000;
            
    }
    /* .menu.scrolled
    {   
        background: #CDE8E8;
        color: white;  
    } */
    ul
    {
        list-style-type:none;
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
    }
    li
    {
        margin: 0 10px;
        color: #628C88;
        padding: 5px;
    }
    li:hover
    {
        background: white;
        padding: 10px;
        border-radius: 50px;
        transition: .5s;
    }
    a
    {
        text-decoration: none;
        color: #628C88;
        font-size: 20px;
    }
    @media (max-width: 1010px)
    {
        a
        {
            font-size: 15px;
            
        }
        li
        {
            padding: 0px;
        }
    }
    @media (max-width: 850px)
    {
        .boton
        {
            position: fixed;
            top: 96%;
            background: linear-gradient(-45deg,#628C88,#CDE8E8,#CDE8E8);
            width: 100%;
            padding: 5px;
            padding: 10px;
        }
        li:hover
        {
            margin: 2px;
            padding: 5px;
        }
        a
        {
            font-size: 20px;
            margin: 0;
        }
    }
    @media(max-width: 450px)
    {
        a{
            font-size: 15px;
        }
    }
    @media (max-width: 400px)
    {
        a
        {
            font-size: 10px;
        }

    }
    
</style>