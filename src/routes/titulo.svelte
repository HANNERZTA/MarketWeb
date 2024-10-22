<script>
    import Img from '../lib/IMG/imgTitulo2.png';
</script>
<div class="container">
    <div class="box">
        <h1 class="titulo">Creación de diseño web y marketing</h1>
    </div>
    <div class="box2">
        <img src={Img} alt="">
    </div>
</div>
<style>
    .container
    {
        display:block;
        position: relative;
        height: 500px;
    }
    .container .box
    {
        margin: 0 auto;
        text-align: center;
        width: 100%;
       
    }
    .container .box2
    {
        position: absolute;
        left: 30%;
        top: 30%;
       
    }
    .titulo
    {
        margin: 10%;
        margin-left: 20%;   
        font-family:Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
        text-transform: uppercase;
        background-image: linear-gradient(-250deg, #CDE8E8 0%, #628C88 50%, #CDE8E8 100%);
        background-size: auto auto;
        background-clip: border-box;
        background-size: 200% auto;
        text-fill-color: transparent;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        animation: bgText 10s linear infinite;
        font-size: 4em; 
    }
    @keyframes bgText {
        to {
            background-position: 200% center;    
        }
    }
</style>