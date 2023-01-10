<template>
    <nav class="navbar navbar-expand-lg bg-transparent">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">
                <img src="https://i.postimg.cc/MGHKvcG0/c-1.gif" alt="logo" style="width:4em">
            </a>
            <button class="navbar-toggler bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
                aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavDropdown">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <router-link to="/"><i class="bi bi-house"></i>Home</router-link>
                    </li>
                    <li class="nav-item">
                        <a href="#about"><i class="bi bi-info-circle-fill"></i>About</a>
                    </li>
                    <li class="nav-item">
                        <a href="#resume"><i class="bi bi-file-earmark-person"></i>Resume</a>
                    </li>
                    <li class="nav-item">
                        <a href="#projects"><i class="bi bi-clipboard-data"></i>Projects</a>
                    </li>
                    <li class="nav-item">
                        <a href="#testimonials"><i class="bi bi-chat-left-quote-fill"></i>Testimonials</a>
                    </li>
                    <li class="nav-item">
                        <a href="#contact"><i class="bi bi-telephone"></i>Contact</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <RouterView/>
</template>

<script>
    export default {
    name: 'NavBar',
    }
</script>

<style scoped>
a {
    text-decoration: none;
    margin: 0 0.5em;
    color: white;
    font-weight: bold;
    text-shadow: 2px 2px 2px black;
    font-size: 20px;
}

a:hover {
    color: rgb(100, 194, 225);
}
</style>