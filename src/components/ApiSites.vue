<template>
    <div class="api-sites">
        <h2>Sites Favoritos</h2>
        <ul>
            <li v-for="site of sitesfavoritos" :key="site.id">
                <a :href="site.link"> {{site.nome}} </a>
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'ApiSites',
    data(){
        return{
            sitesfavoritos: []
        }
    },
    created(){
        fetch (' https://hackthon-decola.firebaseio.com/sites-favoritos.json')
            .then(response => response.json())
            .then (json => {
                this.sitesfavoritos = json;
        });
    }
}
</script>

<style scoped>

</style>
