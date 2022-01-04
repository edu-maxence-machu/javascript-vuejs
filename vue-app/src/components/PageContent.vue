
<template>
<!-- Comment interpréter text="blabla" qui est envoyé depuis le parent ? */-->
    <div>
        <p>{{ numero }}. {{ text }}</p>
  </div>
</template>

<script>
export default {
    props: ['text', 'numero']
}
</script>

<style>

</style>