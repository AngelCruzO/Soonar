<template>
    <header>
        <div class="logo">
            <h1><a href="">Soonar</a></h1>
        </div>
        <nav>
            <li><a href="">Inicio</a></li>
            <li><a href="">Ecosistema</a></li>
            <li><a href="">Voluntariado</a></li>
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
    justify-content: space-between;
    align-items: center;
    background: #3333;
}

nav{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 500px;
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


</style>