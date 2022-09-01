<template>
    <div id="container">
        <div style="background-color: purple; color:white; padding: 80px;">
            <h2>Hello World</h2>
            <h3>Hello there! Just passing by randomly to show this lil test text at home page of this site.</h3>
            <div class="buttons">
                <div class="button1">BUTTON 1</div>
                <div class="button2">BUTTON 2</div>
            </div>
        </div>
        <h2 style="text-align: center; margin: 50px;">Conheça as nossas novidades!</h2>
        <div class="content-produtos">
            <div class="cont-prod">
                <div class="img"></div>
                <div class="prodName">Produto Aleatório</div>
                <div class="prodDesc">Produto Aleatório gerado por uma mente</div>
                <div class="prodPreco">R$ 79,90</div>
                <router-link id="sobre-icon" to="/produto-view">
                    <div class="prodButton">Adicionar ao Carrinho</div>
                </router-link>
            </div>

            <div class="cont-prod">
                <div class="img"></div>
                <div class="prodName">Produto Aleatório</div>
                <div class="prodDesc">Produto Aleatório gerado por uma mente</div>
                <div class="prodPreco">R$ 79,90</div>
                <router-link id="sobre-icon" to="/produto-view">
                    <div class="prodButton">Adicionar ao Carrinho</div>
                </router-link>
            </div>
            <div class="cont-prod">
                <div class="img"></div>
                <div class="prodName">Produto Aleatório</div>
                <div class="prodDesc">Produto Aleatório gerado por uma mente</div>
                <div class="prodPreco">R$ 79,90</div>
                <router-link id="sobre-icon" to="/produto-view">
                    <div class="prodButton">Adicionar ao Carrinho</div>
                </router-link>
            </div>

        </div>
    </div>
</template>
<style>
/* 
body::-webkit-scrollbar {
  width: 10px;
}
body::-webkit-scrollbar-track {
  background-color:#11171a;
position: absolute; 
}
body::-webkit-scrollbar-thumb {
  background-color: #545454;
} */
.buttons {
    display: flex;
    flex-wrap: wrap;
}

.button1,
.button2 {
    font-size: 12px;
    font-weight: 600;
    text-align: center;
    color: white;
    width: 50vh;
    margin-top: 15px;
    margin-bottom: 15px;
    margin-right: 30px;
    cursor: pointer;
    transition: 0.2s;
}

.button1:active {
    background-color: rgb(46, 45, 45);
}

.button2:active {
    background-color: rgba(25, 25, 25, 0.097);
}

.button1 {
    background-color: black;
    padding: 18px;
}

.button2 {
    border: 1px white solid;
    padding: 16px;
}

.content-produtos {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.cont-prod {
    width: 10em;
    margin: 30px;
}

.img {
    height: 12em;
    width: 100%;
    background-color: rgb(181, 179, 179);
    cursor: pointer;
}

.prodName,
.prodDesc,
.prodPreco,
.prodButton {
    text-align: center;
    margin: 18px
}

.prodName {
    font-size: 17px;
    font-weight: 300;

}

.prodDesc {
    font-size: 16px;
    color: grey;
}

.prodPreco {
    font-weight: 800;
    font-size: 16px;
}

.prodButton {
    margin-top: -10px;
    font-size: 14px;
    font-weight: 500;
    padding: 10px;
    border-radius: 5px;
    background-color: black;
    color: white;
    cursor: pointer
}
</style>
<script>
import Button from '.././components/button.vue'
import LateralMenu from '.././components/LateralMenu.vue'
import Registro from '@/components/Registro.vue'

export default {
    name: "Home",
    data() {
        return {
            image: "@/assets/bg-register.png"
        }
    },
    components: { Button, LateralMenu, Registro },
    mounted: function () {
        window.scrollTo(0, 0)
    }
}
</script>
