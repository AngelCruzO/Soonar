<template>
    <header>
        <div class="logo">
            <h1><a href="">Soonar</a></h1>
        </div>
        <nav>
            <ul>
                <li><a href="">Inicio</a></li>
                <li><a href="">Ecosistema</a></li>
                <li><a href="">Voluntariado</a></li>
            </ul>
            
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Menu'
}
</script>

<style>

/* GENERALES */

@font-face {
    font-family: 'Abang Regular';
    font-style: normal;
    font-weight: normal;
    src: local('Abang Regular'), url('../assets/fonts/Abang.woff') format('woff');
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header{
    height: 90px;
    display: flex;
    /* flex-wrap: wrap; */
    justify-content: space-between;
    align-items: center;
    background: #3333;
}

nav{
    
    width: 500px;
}

ul{
    display: flex;
    justify-content: space-around;
    align-items: center;

}

li{
    list-style: none;
}

a{
    text-decoration: none;
}

/* ESPECIFICOS */

.logo{
    font-family: 'Abang Regular';
    font-size: 25px;
    margin-left: 2em;
    color: #7BC789;
}

h1 a{
    color: #7BC789;
}

li a{
    color: #fff;
    font-size: 24px;
}

@media (max-width: 680px) {
    header {
        height: auto;
        width: 100%;
        flex-direction: column;
    }

    .logo{
        margin: 20px;
    }

    ul{
        margin-top: 10px;
        margin-bottom: 20px;
    }
}

</style>