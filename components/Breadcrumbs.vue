<template>
    <div id="Breadcrumbs">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/login">Login</nuxt-link>
        <nuxt-link to="/secret">Secret</nuxt-link>
    </div>
</template>

<script>
export default {
name: "Breadcrumbs"
}
</script>

<style scoped>
#Breadcrumbs{
    background-color:chocolate;
    min-height: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

a{
    color:white;
    font-size: 1.5rem;
    font-weight: bold;
    text-decoration: none;
    transition: all 0.25s;
    margin: 1rem 2.5rem;
}

a:hover{
    border-bottom: 2px black solid;
    color:black;
}
</style>