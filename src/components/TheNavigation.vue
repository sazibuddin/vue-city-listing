<template>
    <nav id="navigation">
         <router-link to="/">Home</router-link>
         <router-link to="/bangladesh">Bangladesh</router-link>
         <router-link to="/brazil">Brazil</router-link>
         <router-link to="/hawaii">Hawaii</router-link>
         <router-link to="/jamaica">Jamaica</router-link>
         <router-link to="/about">About</router-link>
    </nav>
</template>
<style scoped>
#navigation {
    display: flex;
    justify-content: center;
    background: #ccc;
}
.router-link-active {
    color: green;
}
#navigation a {
    padding: 20px 10px;
    text-decoration: none;
    font-weight: bold;
}
</style>
