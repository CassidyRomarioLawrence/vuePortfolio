<template>
    <div>

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
                    year:"2016",
                },
                {
                    name: "Siyaya Skills Institute",
                    qualification: "Business Administration Level 2 & 3",
                    year: "2018 - 2020",
                },
                {
                    name: "College of Cape Town - Crawford",
                    qualification: "CCNA & I.T Essentials",
                    year: "2021",
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
                    year:"2017"
                },
                {
                    name: "Disabled People South Africa(DPSA)",
                    position: "Junior HR & Finance Administrator",
                    year: "2019 - 2020"
                },
                {
                    name: "Oaklands High School",
                    position: "Secretarial Assistant & I.T Support",
                    year: "2022"
                },
            ]
            }
        }
    }
</script>

<style scoped>

</style>