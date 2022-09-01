<template>
    <div>
        <div class="menu" autofocus>
        <div style="display: flex;">
        <a href="/"><div style="color:white; margin-left:7px; margin-top:22px; font-size: 16px;font-weight: 600; text-align: left;">FranRomao.</div></a>
        </div>
                
           
            
            <router-link to="">
                <div v-on:click="menuLateral" class="ham-icon">
                    <div class="line" :class="hamColor"></div>
                    <div class="line lineM" :class="hamColor"></div>
                    <div class="line" :class="hamColor"></div>
                </div>
            </router-link>
            
            <div class="menuLateral" :class="ml_on">
                <LateralMenu />
            </div>

        </div>

    </div>
</template>

<script>
import LateralMenu from './LateralMenu.vue';
export default {
    name: "Nav_bar",
    components: {
        LateralMenu,
    },
    data() {
        return {
            isActive: false,
            hamColor: "",
            ml_on: ""
        }
    },
    methods: {
        menuLateral: function () {
            this.isActive = !this.isActive;
            if (this.isActive == true) {
                this.hamColor = "hamColor";
                this.ml_on = "ml-on"
            }
            else {
                this.hamColor = ""
                this.ml_on = ""
            }
            console.log(this.ml_on)
        }
    }

}

</script>

<style>

.menuLateral {
    position: absolute;
    height: 100vh;
    right: -100%;
    transition: 0.5s;
    opacity: 0;
    top: 64px;
}

.ml-on {
    right: 0;
    opacity: 1;
}

.menu {
    position: fixed;
    display: flex;
    justify-content: space-between;
    background-color: #000;
    margin-top: 0%;
    margin: 0;
    padding: 0;
    width: 100%;
}

.ham-icon {
    padding: 20px;
}

.lineM {
    margin-top: 6px;
    margin-bottom: 6px;
}

.line {
    height: 0.6vh;
    width: 4.5vh;
    border-radius: 00px;
    background-color: #fff;

}

.hamColor {
    background-color: #0ee4b6;
}
.ham-icon:active{
    transform: rotate(180deg);
    transition: 0.5s;
}

#ham-icon,
#sobre-icon {
    padding: 10px;
}

#sobre-icon {
    text-decoration: none;
    color: rgb(227, 225, 225);
    margin-top: 5px;
    margin-right: 5px;
    font-size: 14px;
    font-weight: lighter;
}
</style>
