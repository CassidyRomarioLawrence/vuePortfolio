<template>
    <div class="container pro-cards text-center justify-content-center">
        <!-- <div class="row">
            <div v-for="item in projects" :key="item" class="card m-3" style="width: 18rem;">
                <img :src="item.img" alt="Image">
                <div class="container">
                    <h4 class="Title">{{ item.name }}</h4>
                    <a :href=item.links.github target="_blank"><button>GitHub</button></a>
                    <a :href=item.links.netlify target="_blank"><button>Netlify</button></a>
                </div>
            </div>
        </div> -->
    </div>
</template>

<script>
    export default {
    name: 'ProjectsComponent',
    data() {
        return {
            projects: [
                {
                    name: "JavaScript Site",
                    img: "",
                    links: {
                        github: "",
                        netlify: ""
                    }
                },
                {
                    name: "JavaScript Calculator",
                    img: "https://i.postimg.cc/mkFy7d2F/calculator-Project.png",
                    links: {
                        github: "",
                        netlify: "https://cassidy-calculator.netlify.app/"
                    }
                },
                {
                    name: "HTML&CSS Portfolio",
                    img: "",
                    links: {
                        github: "",
                        netlify: ""
                    }
                },
                {
                    name: "HTML&CSS Ecommerce Site",
                    img: "https://i.postimg.cc/pdJWLxfm/Ecommerce-Project.png",
                    links: {
                        github: "",
                        netlify: ""
                    }
                },
                {
                    name: "HTML&CSS Dog Sitter Site",
                    img: "https://i.postimg.cc/nVvkVP56/Dog-Sitter-Project.png",
                    links: {
                        github: "",
                        netlify: ""
                    }
                },
                {
                    name: "",
                    img: "",
                    links: {
                        github: "",
                        netlify: ""
                    }
                },
            ]
        }
    }
    }
</script>

<style scoped>
.card{
    background-color: rgb(220, 214, 214);
}
button {
    padding: 4px;
    background-color: black;
    color: white;
    border-radius: 4px;
    cursor: pointer;
}
</style>