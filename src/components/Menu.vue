<template>
    <header>
        <div class="logo">
            <h1><a href="">Soonar</a></h1>
        </div>
        <nav>
            <ul>
                <li><a href="" data-text="Inicio">Inicio</a></li>
                <li><a href="" data-text="Ecosistema">Ecosistema</a></li>
                <li><a href="" data-text="Voluntariado">Voluntariado</a></li>
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

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@800&display=swap');

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
    /* background: #3333; */
}

nav{    
    width: 500px;
    margin-right: 20px;
    font-family: 'Poppins', sans-serif;
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
    font-family: 'Abang Regular',sans-serif;
    font-size: 25px;
    margin-left: 2em;
    color: #7BC789;
}

h1 a{
    color: #7BC789;
}

ul li a{
	position: relative;
	display: block;
	text-decoration: none;
	font-size: 25px;
	font-weight: 800;
	color: rgba(255, 255, 255, 0.5);
    /* text-shadow: 0 0 10px rgba(0, 0, 0, 0.2); */
}

ul li a:before{
	content: attr(data-text);
	position: absolute;
	top: 0;
	left: 0;
	background: url(../assets/wave.png);
	-webkit-background-clip: text;
	background-repeat: repeat-x;
	animation:  animate 2s linear infinite;
	transition: 0.5s;
	width: 0;
	overflow: hidden;
	white-space: nowrap;
}

ul li a:hover:before{
	width: 100%;
}

@keyframes animate{

	0%{
		background-position: 0px;
	}

	100%{
		background-position: 200px;
	}

}

@media (max-width: 800px) {
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