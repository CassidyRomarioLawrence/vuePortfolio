<template>
    <div class="container my-cards text-center justify-content-center">
        <!-- <div class="row">
                <div v-for="item in testimonials" :key="item" class="card m-3" style="width: 18rem;">
                    <img :src=item.img class="card-img-top test-img" alt="persons-image">
                    <div class="card-body">
                        <h5 class="card-title">{{ item.fullName }}</h5>
                        <h6>{{ item.position }}</h6>
                        <p>{{ item.msg }}</p>
                    </div>
                </div>
        </div> -->
    </div>
</template>

<script>
    export default {
    name: 'TestimonialComponent',
    data() {
        return {
            testimonials: [
                {
                    fullName: "Sive Shabane",
                    position:"Peer",
                    img: "https://i.postimg.cc/t43Rtkhx/Sive-profile.png",
                    msg:"Cassidy is very dedicated in his work. He remains fully focused on the task at hand till completion.He is a great team player and always willing to help whenever his expertise is called upon.He is very respectful and understanding of everyone around him and creates an excellent work environment.He would make a wonderful addition to any team he is placed within and up for a challenge.",
                },
                {
                    fullName: "Joel Mukanya",
                    position: "Lecturer",
                    img: "https://i.postimg.cc/WzkTgWbx/Joel-Profile.jpg",
                    msg: "Cassidy is a very creative, go-getter, and well-behaved student. He does enjoy working with his classmates and works well on his project.He has gained knowledge of web development, including Bootstrap 5. I will be very delighted to see him get hired as a developer.",
                },
                {
                    fullName: "Meezaan Davids",
                    position: "Peer",
                    img: "https://i.postimg.cc/Kj7F00CV/Screenshot-20221105-101408.png",
                    msg: "Cassidy is a very smart and open minded guy. He has a keep to himself character but once engaging in conversations, he genuinely has such good takes on different aspect of things.He has a lot of skills varying from football to coding which I personally think can only get better.Cassidy will go very far in life with his open minded mentality and I'm sure will be a great success.",
                },
                {
                    fullName: "Mu-een Slamat",
                    position: "Peer",
                    img: "https://i.postimg.cc/6QDXtsXg/Screenshot-20221105-094654.png",
                    msg: "Cassidy has been a good friend of mine for 2 years and I can honestly say that he is open-minded ,friendly,funny,hard working, humble and a genuine person.He never hesitates to help out the next person.He is goal driven.He will always try his best to solve a problem and never struggles to ask for help if needed.His creative side almost never disappoints.Once he sets his mind to solve a task, he gets it done.",
                },
                {
                    fullName: "Brogan Gys",
                    position: "Peer",
                    img: "https://i.postimg.cc/zG5HDWxq/Brogan-Profile.jpg",
                    msg: "Cassidy is someone who always sticks to the task at hand, and gives 100% to all his tasks / projects.He has great social skills making a good team player, he is a smart and knowledgeable guy that always has good advice to offer to any one that seeks it.",
                },
                {
                    fullName: "Asandile Langeni",
                    position: "Peer",
                    img: "https://i.postimg.cc/0jM2Z5ZW/DSC-3626.jpg",
                    msg: "Cassidy is a reliable friend, he is joyful to be around. He likes learning about new stuff, he would go learn new thing and come to discuss with us in order to help us get the knowledge he has. He is hard working furthermore he is a team player that knows how to accommodate everyone. Cassidy is always smiling and if he is not, he is making sure that those who around him smile.",
                },
            ]
            }
        }
    }
</script>

<style scoped>
.test-img{
    border-radius: 8px;
    padding: 4px 0;
}
.card{
    background-color: rgb(220, 214, 214);
}
.card-title{
    font-weight: bold;
    animation: fun;
    animation-duration: 4s;
    animation-iteration-count: infinite;
}

@keyframes fun {
    0% {
        color: black;
    }

    25% {
        color: purple;
    }

    50% {
        color: lightcoral;
    }

    75% {
        color: lightseagreen;
    }

    100% {
        color: lightgreen;
    }
}
</style>