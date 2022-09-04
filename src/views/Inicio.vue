<template>
    <section>
        <Menu/>
        <video src="../assets/fondo.mp4" muted loop autoplay></video>
        <div class="overlay"></div>
        <div class="content">
            <h1>Inicio</h1>
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
    :root{
        --overlay-color: #03a9f4
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
        justify-content: center;
        align-items: center;
        height: 80vh;
    }

</style>