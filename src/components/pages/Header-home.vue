<!-- Componente de header da página home -->
<template>
    <header>
        <b-navbar toggleable="md" type="dark" variant="dark">
            <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
            <b-navbar-brand href="/">CurriculoIncit</b-navbar-brand>

            <b-collapse is-nav id="nav_collapse">
                <b-navbar-nav>
                    <b-nav-item href="/">Início</b-nav-item>
                </b-navbar-nav>
            </b-collapse>                                

            <b-navbar-nav class="ml-auto">
                <div id="loginButton" >
                    <b-btn variant="light" @click="redirectLogin">Login</b-btn>                    
                </div>
            </b-navbar-nav>
            
        </b-navbar>
    </header>
</template>

<script>
export default {
    name: "headerHome",
    methods: {
        redirectLogin () {
            this.$router.push('/login');
        }
    },
};
</script>
