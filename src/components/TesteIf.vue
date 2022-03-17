<template>
    <div class="Teste-if">
        <h1 v-if = "podeVer"> Teste v-if </h1>
        <h2 v-else>Teste v-else</h2>

    </div>
</template>

<script>
export default {
    name: 'TesteIf',
    data(){
        return {
            podeVer: true

        }
    }
}
</script>

<style scoped>

</style>
