<template>
    <nav>
        <div class="nav-container">
            <img src="@/assets/logo.png" alt="">
            <div id="link-list">
                <a href="#home" class="active">Inicio</a>
                <a href="#about-us">Sobre nosotros</a>
                <a href="#our-team">Nuestro equipo</a>
                <a href="#our-project">Nuestro proyecto</a>
            </div>
        </div>
    </nav>
</template>

<style scoped>
    nav {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        background-color: rgba(245, 245, 245, 0.3);
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        z-index: 10;
    }
    
    nav .nav-container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1rem;
    }

    nav .nav-container img {
        display: block;
        max-height: 50px;
    }

    nav .nav-container #link-list {
        display: flex;
    }

    nav .nav-container #link-list a {
        margin: 0 1rem;
        color: #819dbb !important;
        font-weight: 500;
        text-decoration: none;
        transition: color 0.2s;
    }

    nav .nav-container #link-list a.active, nav .nav-container #link-list a:hover {
        color: #2c3e50 !important;
    }
</style>

<script>
export default {
    name: 'Navbar',
    components: {
    }
}
</script>