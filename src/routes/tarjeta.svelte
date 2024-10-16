<div class="container">
    <div class="tarjetas">
        <div class="redes">
            <i class="fa-brands fa-square-facebook"></i>
            <i class="fa-brands fa-square-instagram"></i>
            <i class="fa-brands fa-square-whatsapp"></i>
        </div>
        <div class="foto"></div>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod
            distinctio in eius magni blanditiis, quaerat error nemo voluptates
            earum voluptate explicabo eaque debitis dignissimos ducimus. Qui quo
            labore nobis dolores?
        </p>
    </div>

    <div class="tarjetas">
        <div class="redes">
            <i class="fa-brands fa-square-facebook"></i>
            <i class="fa-brands fa-square-instagram"></i>
            <i class="fa-brands fa-square-whatsapp"></i>
        </div>
        <div class="foto"></div>
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nobis
            consequuntur placeat inventore ab itaque quod ad explicabo laborum
            iusto delectus? Quas earum veritatis quidem ab quisquam, beatae rem
            cumque doloribus?
        </p>
    </div>
    <div class="tarjetas">
        <div class="redes">
            <i class="fa-brands fa-square-facebook"></i>
            <i class="fa-brands fa-square-instagram"></i>
            <i class="fa-brands fa-square-whatsapp"></i>
        </div>
        <div class="foto"></div>
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Excepturi
            eius dignissimos, rem et ratione commodi distinctio error! Dolor,
            ex? Minima molestias veritatis cumque, molestiae omnis odio ratione
            animi labore quasi!
        </p>
    </div>
</div>

<style>
    .container {
        display: flex;
    }
    .tarjetas {
        background: linear-gradient(
            45deg,
            #cde8e8 0%,
            #628c88 50%,
            #cde8e8 100%
        );
        width: 25%;
        margin: 5%;
        text-align: center;
        border-radius: 10px;
        box-shadow: 5px 5px 20px black;
        position: relative;
    }
    .foto {
        margin: 0 auto;
        margin-top: 20px;
        background: black;
        width: 50%;
        height: 130px;
        border-radius: 50%;
    }
    p {
        margin: 20px;
    }
    .redes {
        text-align: center;
        position: absolute;
        right: 0%;
        top: 3%;
        display: none;
        background: rgba(184, 190, 186, 0.432);
        width: 40px;
        border-radius: 10px;
    }
    i {
        width: 50%;
        margin: 0 auto;
        font-size: 25px;
        margin: 5px;
        color: #6b6b6b;
    }

    .tarjetas:hover .redes
    {
        display: block;
    }
</style>
