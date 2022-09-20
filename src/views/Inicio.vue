<template>
    <section>
        <Menu/>
        <video src="../assets/fondo.mp4" muted loop autoplay></video>
        <div class="overlay"></div>
        <div class="content">
            <h1 class="title">Nuestro Hogar</h1>
            <p class="somos">
                La generación de basura es acumulada en grandes sumas a diario y gran cantidad de las mismas
                terminan en zonas fluviales, mares y océanos; ya sea al drenar áreas urbanas o mediante la tira 
                de residuos humanos como envolturas y desechos. Este producto pone en peligro la vida de la flora y 
                fauna marina de manera directa como en la ingesta de residuos plásticos, así como cambios en los ecosistemas, 
                causa de la exposición prolongada a los mismos, generadndo modificaciones de PH en el agua a la propagación 
                de especies por mitovos de migración forzada y reproducción anormal de organismos invasivos como es el caso particular del ssargazo
                <br><br>
                El único proyecto hasta ahora para recapturar los desechos plásticos en el océano no hace lo que se supone que debe hacer, 
                desafortunadamente, no se acumulan los residuos solamente en la superficie. Estudios anteriores habían encontrado que incluso 
                el plástico flotante es empujado regularmente muy por debajo de la superficie por el viento y la turbulencia.
                <br><br>
                Es por eso que te proponemos un trato, ayúdanos a mantener nuestro primer hogar recogiendo los residuos que encuentres y cámbialos
                por puntos caracolas. Junta suficientes y canjéalos por productos. Esto nos permitirá mantener nuestros océanos limpios y conseguir
                más meterial para seguir otorgándote productos de calidad. O, si necesitas empleo temporal tambén pudes acercarte a nosotros y te 
                canalizaremos a proyectos de recolección de sargazo y capacitación para la preparación de productos con nuestros colaboradores.
            </p>
        </div>
    </section>
</template>

<script>
    import Menu from '@/components/Menu.vue'
    export default {
        name: 'Inicio',
        components:{
            Menu
        }
    }
</script>

<style>
    @font-face {
        font-family: 'Abang Regular';
        font-style: normal;
        font-weight: normal;
        src: local('Abang Regular'), url('../assets/fonts/Abang.woff') format('woff');
    }

    :root{
        --overlay-color: #03a9f4;
    }

    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    section video{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        opacity: 0.9;
        z-index: -1;
    }

    .overlay{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: var(--overlay-color);
        mix-blend-mode: overlay;
        z-index: -1;
    }

    .content{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 80vh;
    }

    .title{
        font-family: 'Abang Regular', sans-serif;
        font-size: 65px;
        margin-bottom: 20px;
    }

    .somos{
        font-family: 'Poppins', sans-serif;
        font-size: 18px;
        width: 75%;
        text-align: justify;
        /* background: rgba(255, 255, 255, 0.2); */
    }
</style>