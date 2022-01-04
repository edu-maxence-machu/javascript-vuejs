<script>
import MenuLink from './MenuLink'; 
    
export default {  
    name: 'Menu',
    components: {
        MenuLink
    }
}
</script>

<template>
    <div>
        <MenuLink url="/" active="false" text="Home"/>
        <MenuLink url="/cv" active="true" text="CV"/>
        <MenuLink url="/contact" active="true" text="Contactez-moi"/>
    </div>
</template>

<style lang="scss" scoped>

    * {
        font-family: sans-serif;
    }

    a {
        text-decoration: none;

        &:hover {
            opacity: 0.7;
        }
    }
</style>