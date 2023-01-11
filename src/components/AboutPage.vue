<template>
    <div class="container-fluid about">
        <div class="row">
        </div>
        <div class="row">
            <div class="col-xs-12 col-md-6 col-lg-6">
                <img class="my-image img-fluid" src="https://i.postimg.cc/W4BGz9ts/Profile.png" alt="profile-photo" />
            </div>
            <div class="col-xs-12 col-md-6 col-lg-6 d-flex align-items-center">
                <p class="lead text-center p-3 para">
                    My name is Cassidy Romario Lawrence, I'm a 24-year-old male currently
                    studying coding <br />
                    at Life Choices Academy. <br /><br />
                    I come from Rocklands Mitchell's Plain. <br />
                    My hobbies include playing video games, soccer and working out
                    occasionally. <br /><br />
                    I am a friendly individual, always up for new challenges. <br />I
                    always aspire to be a great team player. <br />I possess the ability
                    to work unsupervised, <br />I'm trustworthy, goal driven, punctual and
                    well-mannered. <br />I'm always eager to sharpen skills I've already
                    acquired. <br />
                    As well as learning new ones to improve myself and grow my skill set.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'AboutPage'
    }
</script>

<style scoped>
.para{
    font-weight: bold;
}
.my-image {
    border-radius: 4px;
    border: 2.5px solid white;
    width: 30rem;
}
.col-xs-12 {
    text-align: center;
    margin-left: auto;
    margin-right: auto;
}
</style>