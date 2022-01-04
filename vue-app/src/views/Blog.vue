<template>
    <div class="blog__article">
        <h1>Hello blog: {{ title }} </h1>
    </div>
</template>

<script>
export default {
        data() { 
            return {title: "Titre de l'article" }
        },
        beforeCreate() { console.log('Je ne suis pas encore  créé') },
        created() { console.log('Je suis créé !') },
        beforeMount() { console.log('Je vais bientôt être monté sur le DOM!') },
        mounted() { console.log('Je suis monté sur le DOM!') },
        beforeUnmount() { console.log('Je suis sur le point de disparaître du DOM !') },
        unmounted() { console.log('Je suis supprimé') }
}
</script>

<style>

</style>