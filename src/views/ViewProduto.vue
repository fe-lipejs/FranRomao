<template>
    <div class="card"></div>
    <div>
        <div class="info">
            <div class="info-product">Relógio Orient 323L</div>
            <div class="info-desc">Este é um relógio mega fictício onde estou escrevendo este enorme, porém parcial
                texto para encher línguiça nessa parte de teste do site de vendas.</div>
            <div class="info-price-cores">
                <div class="info-price">R$ 179</div>
                <div class="cores">
                    <div class="color color1 "></div>
                    <div class="color color2  color-selected"></div>
                    <div class="color color3"></div>
                </div>
            </div>
        </div>
        <a href="/card-produto"><div class="button">Continue</div></a>
    </div>
</template>


<style>
div {
    color: black;
}

.card {
    background-color: rgb(223, 222, 222);
    height: 15em;
    width: 100%;
    text-align: center;
}

.info {
    margin-top: 30px;
    margin: 16px;
}

.info-price-cores {
    display: flex;
    justify-content: space-between;
    margin-top: 30px;
}

.info-product {
    font-weight: 800;
    font-size: 30px;
    text-align: left;
}

.info-desc {
    margin-top: 20px;
    color: rgb(58, 57, 57);
    font-size: 17px;
    text-align: left;

}

.info-price {
    text-align: left;
    font-weight: 1000;
    font-size: 25px;
    margin-top: 3px;
}

.cores {
    display: flex;
}

.color1 {
    background-color: burlywood;
}

.color2 {
    background-color: rgb(150, 42, 42);
}

.color3 {
    background-color: rgb(44, 42, 42);
}

.color {
    margin: 5px;
    width: 1em;
    height: 1em;
    border-radius: 100%;
    cursor: pointer;
}

.color-selected {
    outline: 2px solid rgb(113, 111, 111);
    border: 2px solid #eee;
    margin-top: 0.5px;

}

.button {
    text-align: center;
    background-color: rgb(26, 25, 25);
    margin-top: 30px;
    padding: 10px;
    width: 200px;
    cursor: pointer;
    margin-left: -20px;
}

.button:active {
    background-color: rgb(1, 40, 43);

}

.button span {
    color: white;
    font-size: 20px;
    font-weight: 50;
}
</style>

<script>
export default {
    components:{

    },
    mounted: function(){
      window.scrollTo(0,0)  
    },
    data() {
        return {
            
        }
    },

}
</script>