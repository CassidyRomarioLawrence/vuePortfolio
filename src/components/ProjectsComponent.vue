<template>
    <div class="container my-projects">
                <div v-for="item in projects" :key="item" class="card my-2" style="width: 18rem;">
                    <img class="card-img-top" :src=item.img alt="Card image cap" />
                    <div class="card-block text-center">
                        <h4 class="card-title">{{ item.name }}</h4>
                        <a :href=item.links.github target="_blank" class="card-link"><button class="btn"><i
                                    class="bi bi-github"></i>GitHub</button></a>
                        <a :href=item.links.netlify target="_blank" class="card-link"><button class="btn"><i
                                    class="bi bi-globe"></i>Netlify</button></a>
                    </div>
                </div>
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
                    img: "https://i.postimg.cc/pTpvKyM0/Eccomerce-Java-Project.png",
                    links: {
                        github: "",
                        netlify: "https://lawrencecassidyeompjs.netlify.app/"
                    }
                },
                {
                    name: "JavaScript Calculator",
                    img: "https://i.postimg.cc/mkFy7d2F/calculator-Project.png",
                    links: {
                        github: "https://github.com/CassidyRomarioLawrence/CalculatorYouNeed",
                        netlify: "https://cassidy-calculator.netlify.app/"
                    }
                },
                {
                    name: "HTML&CSS Portfolio",
                    img: "https://i.postimg.cc/kXDj98FY/HTML-CSS-portfolio.png",
                    links: {
                        github: "https://github.com/CassidyRomarioLawrence/updatedPort",
                        netlify: "https://cassidylawrence-portfolio.netlify.app/"
                    }
                },
                {
                    name: "HTML&CSS Ecommerce Site",
                    img: "https://i.postimg.cc/pdJWLxfm/Ecommerce-Project.png",
                    links: {
                        github: "https://github.com/CassidyRomarioLawrence/Ecommerce",
                        netlify: "https://ecommerce-practice-run.netlify.app/"
                    }
                },
                {
                    name: "HTML&CSS Dog Sitter Site",
                    img: "https://i.postimg.cc/nVvkVP56/Dog-Sitter-Project.png",
                    links: {
                        github: "https://github.com/CassidyRomarioLawrence/Dog-Sitter",
                        netlify: "https://dog-sitter-site.netlify.app/"
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
.my-projects{
    display: flex;
    justify-content: center;
    gap: 0 2rem;
    flex-wrap: wrap;
}
</style>