<template>
    <div class="content-cart">
        <h2>Carrinho de Compras</h2>
        <div class="cart">
            <div class="item">
                <div class="prod-image"></div>
                <div class="prod-nome-frete">
                    <div class="prod-nome">Relógio Cassio L1</div>
                    <div class="prod-frete">Frete: R$ 40,00</div>
                </div>
                <div class="prod-preco">R$ 169</div>
            </div>
            <div class="item">
                <div class="prod-image"></div>
                <div class="prod-nome-frete">
                    <div class="prod-nome">Relógio Cassio L1</div>
                    <div class="prod-frete">Frete: R$ 40,00</div>
                </div>
                <div class="prod-preco">R$ 169</div>
            </div>
            <div class="item">
                <div class="prod-image"></div>
                <div class="prod-nome-frete">
                    <div class="prod-nome">Relógio Cassio L1</div>
                    <div class="prod-frete">Frete: R$ 40,00</div>
                </div>
                <div class="prod-preco">R$ 169</div>
            </div>

            <hr>
            <div class="desc">
                <div class="desc-subtotal">
                    <div class="desc-subtotal-nome">Subtotal</div>
                    <div>R$ 507,00</div>
                </div>
                <div class="desc-frete">
                    <div class="desc-frete-nome">Frete</div>
                    <div>R$ 120,00</div>
                </div>
            </div>
            <hr>
            <div class="total">
                <div class="total-tl">Total</div>
                <div class="total-pc">R$627,00</div>
            </div>
            <div class="button">Continue</div>
        </div>
    </div>
</template>


<style>
body{
    background-color: white;
}
.content-cart h2{
    color:black
    ;text-align: center;
    padding: 70px;
   
}
hr {
    margin-top: 40px;
    height: 1px;
    background-color: rgb(234, 233, 233);
    border: none;
}

.content-cart{
    padding-top: 20px;
}
.item {
    display: flex;
    justify-content: space-evenly;
    margin-bottom: 30px;
    
}

.prod-image {
    background-color: rgba(244, 244, 244, 0.692);
    height: 3em;
    width: 3em;
    border-radius: 10px;
    box-shadow: 3px 2px 5px rgba(208, 206, 206, 0.713);
}

.prod-nome {
    font-weight: 700;
    font-size: 18px;
    margin-top: 10px;
    color: rgb(72, 71, 71);
}

.prod-frete {
    font-weight: 400;
    font-size: 15px;
    color: rgb(153, 151, 151);
    text-align: left;
}

.prod-preco {
    font-weight: 700;
    font-size: 18px;
    margin-top: 10px;
}

.desc-subtotal,
.desc-frete,
.total {
    display: flex;
    justify-content: space-between;
    margin: 30px;
    font-weight: 700;
    font-size: 18px;
    margin-top: 10px;
}

.desc-subtotal-nome,
.desc-frete-nome {
    color: rgb(149, 149, 149);
}

.total {
    margin-top: 30px;
    margin-bottom: 70px;
}

.total-pc {
    font-size: 25px;
}

.button {
    background-color: rgb(26, 25, 25);
    margin: 20px;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
    color: white;
    font-size: 20px;
    font-weight: 50;
}

.button:active {
    background-color: rgb(1, 40, 43);

}
</style> 

<script>
export default {

}
</script>