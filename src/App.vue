<script>
    //Versión 2.0
    /* export default{
        data(){
            return{
                contador: 200,
            };
        },
    }; */

    export default{
        data: () => ({
            contador : 500,
        }),

        methods:{
            saludar(){
                console.log("Hola 10A | @");
            },

            incrementar(){
                this.contador ++;
            },

            decrementar(){
                this.contador --;
            },

            resetear(){
                this.contador = 500;
            },
        }
    };
</script>

<template>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" 
    integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">
    
    <div class="container"> 
        <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
    </div>

    <div class="box">
        <nav class="navbar navbar-dark bg-primary">
            <a class="navbar-brand">Federico Francisco Manuel   9°A  DMI</a>
        </nav>
    </div>

    
    <div class="container">    
        <small>
            <h1>Hola desde VUE.js 3</h1>
        </small>
        <hr>
        <h2>Contador {{ contador }}</h2>
        <button @:click="incrementar()">+1</button>
        <button @click="decrementar()">-1</button>
        <button @click="resetear()">Reset</button>
    </div>
</template>

<style scoped>
    .container{
        text-align: center;
    }

    small{
        color: #666;
    }

    h1{
        font-weight: bolder;
    }

    h2{
        font-size: 2.5rem;
    }

    button{
        cursor: pointer;
        font-size: 1.5rem;
        margin: 0px 8px;
    }
</style>