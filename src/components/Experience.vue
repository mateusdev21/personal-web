<template>
    <section class="p-8 bg-black">
        <h2 class="text-4xl font-extrabold mb-8 text-white">Work Experience</h2>
        <ul class="space-y-4">
            <li class="p-4 border rounded shadow dark:border-gray-700" v-for="(experience, index) in experiences" :key="index">
                <h3 class="text-lg font-medium text-white">{{ experience.position }}</h3>
                <p class="text-sm font-bold text-white">{{ experience.company }} | {{ experience.year }}</p>
                <p class="text-sm text-white">{{ experience.description }}</p>
            </li>
        </ul>
    </section>
</template>
<script setup lang="ts">
const experiences = [
    {
        position: "Frontend Developer",
        company: "PT. Lentera Sinyal Nusantara",
        year: "September 2022 - April 2024",
        description: "Builds and implements user-facing features of websites and applications using HTML, CSS, JavaScript, Typescript, and NuxtJS frameworks. Ensure responsive design and optimal performance. Collaborating with designers and backend developers, translate UI/UX designs into functional code for seamless and interactive user experiences.",
    },
    {
        position: "Frontend Developer",
        company: "CV. Lumintu Logic",
        year: "June 2021 - December 2021",
        description: "Creating and implementing interactive, user-friendly web interfaces using HTML, CSS, JavaScript, JQuery, and PHP. Ensure responsive design, optimize website performance, and ensure cross-browser compatibility. Collaborating with designers and backend teams, they deliver visually appealing, functional, and efficient web applications.",
    },
    {
        position: "UI/UX Designer",
        company: "Freelance",
        year: "January 2021 - May 2021",
        description: "Design user-friendly interfaces using Figma, conduct research, create wireframes/prototypes, improve user experience, and ensure visually appealing, functional digital products.",
    },
    {
        position: "Frontend Developer",
        company: "Freelance",
        year: "December 2020 - May 2021",
        description: "Develops UI using VueJS 2 and Vuetify. ensure responsive, visually appealing designs and seamless user experiences. Responsibilities include optimizing performance, debugging, collaborating with designers and backend teams, and staying updated with emerging technologies to deliver modern, scalable, and efficient web solutions.",
    },
    {
        position: "Wordpress Developer",
        company: "Freelance",
        year: "July 2020 - December 2020",
        description: "Design, develop, and customize WordPress websites, optimize performance, troubleshoot issues, and manage updates.",
    },
    {
        position: "IT Support",
        company: "PT. Mitra Elga Prima",
        year: "June 2018 - May 2020",
        description: "Provide technical support, troubleshoot hardware/software issues, manage IT systems, maintain networks, assist users, and ensure smooth technology operations.",
    },
];
</script>