<template>
  <a :href="url" :class="active ? 'active' : ''">
      {{ text }} {{ exemplePropsComputed }}
  </a>
</template>

<script>
export default {
    name: 'MenuLink',
    props: ['url', 'text', 'active'],
    computed: {
        exemplePropsComputed(){
            return '(' + this.url + ')';
        }
    }
}
</script>

<style lang="scss">
    a {
        &.active {
          font-weight: bold;
        }
    }
</style>