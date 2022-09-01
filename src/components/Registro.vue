<template>
    <div class="content">
        <div>
            <p>
                Neste momento as vagas para o curso
                <span style="color: #de316b; font-weight: 700;">Manicure Russa</span> estão esgotadas,
                preencha os dados abaixo para receber todas as 
                informações da próxima turma.
            </p>
        </div>
        <div class="formulario">
            <div><input type="text" placeholder="Nome completo" name="nome" id=""><br>
            <input type="text" placeholder="Email" name="email" id=""><br>
            <input type="text" placeholder="Telefone com DDD" name="telefone" id=""><br>
            </div><a>QUERO RECEBER INFORMAÇÕES</a>
        </div>
    </div>
</template>
<style>
.content{
    padding:20px;
    
}
.content div p {
    color: rgb(215, 215, 215);
    font-size: 0.7em;
    text-align: center;
    margin: 30px;

}
.content div input::placeholder{
    color: #827e7f; 
    font-weight: 600;
 
}
.formulario div{
    padding-top: 20px;
    padding-bottom: 30px;

}.formulario a{
    margin-top: -20px;
    font-size: 16px;
    font-weight:700;
    cursor: pointer;
    
}
.content div input{
    color: #de316b;
    font-weight: 700;
    width: 80%;
    padding: 0.7em;
    margin-bottom: 1em;
    border-radius: 10px;
    border: 1px solid rgba(104, 74, 84, 0.626);
    background: transparent;

}

</style>
<script>
import Button from './button.vue';
export default {
    components: { Button }
}
</script>