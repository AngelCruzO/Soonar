<template>
    <section>
        <Menu/>
        <video src="../assets/fondo.mp4" muted loop autoplay></video>
        <div class="overlay"></div>
        <div class="center">
            <MainText/>
        </div>
    </section>
</template>

<script>
    import Menu from '@/components/Menu.vue'
    import MainText from '@/components/MainText.vue'
    export default {
        name: 'Inicio',
        components:{
            Menu,
            MainText
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

    .center{
        display: flex;
        justify-content: center;
        align-items: center;
    }

    section video{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        opacity: 0.8;
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
        opacity: 0.7;
    }
</style>