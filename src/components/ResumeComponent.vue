<template>
    <div class="container my-education">
        <h3 class="display-3 text-center">My Education:</h3>
        <table class="table education table-hover table-light">
            <thead>
                <tr>
                    <th scope="col">Institution</th>
                    <th scope="col">Qualification</th>
                    <th scope="col">Year</th>
                </tr>
            </thead>
            <tbody v-for="item in education" :key="item">
                <tr>
                    <td>{{ item.name }}</td>
                    <td>{{ item.qualification }}</td>
                    <td>{{ item.year }}</td>
                </tr>
            </tbody>
        </table>
    </div>

    <div class="container my-work justify-content-center">
        <h3 class="display-3 text-center">My Experience:</h3>
        <table class="table work table-hover table-light">
            <thead>
                <tr>
                    <th scope="col">Organizatiion</th>
                    <th scope="col">Position</th>
                    <th scope="col">Year</th>
                </tr>
            </thead>
            <tbody v-for="item in workExperience" :key="item">
                <tr>
                    <td>{{ item.name }}</td>
                    <td>{{ item.position }}</td>
                    <td>{{ item.year }}</td>
                </tr>
            </tbody>
        </table>
    </div>

    <div class="container my-skills justify-content-center">
        <h3 class="display-3 text-center">My Skills:</h3>
        <table class="table skills table-hover table-light">
            <thead>
                <tr>
                    <th scope="col">Soft Skills</th>
                    <th scope="col">Technical Skills</th>
                </tr>
            </thead>
            <tbody v-for="item in skills" :key="item">
                <tr>
                    <td>{{ item.softSkills.name }}</td>
                    <td>{{ item.techSkills.name }}</td>
                </tr>
            </tbody>
        </table>
    </div>
    
</template>

<script>
    export default {
    name: 'ResumeComponent',
    data() {
        return {
            education: [
                {
                    name: "Rocklands High School",
                    qualification: "Matric Certificate",
                    year:2016,
                },
                {
                    name: "Siyaya Skills Institute",
                    qualification: "Business Administration Level 2 & 3",
                    year: "2018 - 2020",
                },
                {
                    name: "College of Cape Town - Crawford",
                    qualification: "CCNA & I.T Essentials",
                    year: 2021,
                },
                {
                    name: "Life Choices Academy",
                    qualification: "Web Development and Programming",
                    year: "Currently",
                },
            ],
            workExperience: [
                {
                    name: "PEP Stores",
                    position: "General Assistant",
                    year:2017
                },
                {
                    name: "Disabled People South Africa(DPSA)",
                    position: "Junior HR & Finance Administrator",
                    year: "2019 - 2020"
                },
                {
                    name: "Oaklands High School",
                    position: "Secretarial Assistant & I.T Support",
                    year: 2022
                },
            ],
            skills: [
                {
                    softSkills: {
                        name:"Communication Skills"
                    },
                    techSkills: {
                        name:"HTML5"
                    },
                },
                {
                    softSkills: {
                        name: "Time Management Skills"
                    },
                    techSkills: {
                        name: "CSS3"
                    },
                },
                {
                    softSkills: {
                        name: "Administrative Skills"
                    },
                    techSkills: {
                        name: "Bootstrap5"
                    },
                },
                {
                    softSkills: {
                        name: "Customer Service"
                    },
                    techSkills: {
                        name: "JavaScript"
                    },
                },
                {
                    softSkills: {
                        name: "Teamwork"
                    },
                    techSkills: {
                        name: "Vue.js"
                    },
                },
            ]
            }
        }
    }
</script>

<style scoped>
.education,.work,.skills{
    text-shadow:2px 2px 2px rgb(100, 194, 225);
}

thead{
    border-bottom: 2px solid black;
}
</style>