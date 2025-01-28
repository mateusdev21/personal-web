<template>
    <section id="projects" class="p-8 text-center bg-[#fce301]">
        <h2 class="text-4xl font-extrabold mb-8 text-black">PROJECTS</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            <div class="p-4 border rounded shadow" v-for="(project, index) in projects" :key="index">
                <img :src="project.screenshot" alt="" class="h-46 w-96 mb-4 rounded-md">
                <h3 class="text-lg font-medium">{{ project.name }}</h3>
                <p class="text-sm">{{ project.description }}</p>
                <a :href="project.link" target="_blank"
                    class="text-blue-500 hover:underline text-sm mt-2 inline-block">View Project</a>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
const projects = [
    {
        name: "Personal Website",
        description: "This is my personal website for the purpose of displaying my professional experience and what projects I have worked on. I built this website using the Vue JS 3 Frontend Framework and Tailwind as the UI Framework.",
        screenshot: "@/assets/personal-web.png",
        link: "#",
    },
    {
        name: "ETLE Nasional",
        description: "ETLE (Electronic Traffic Law Enforcement) is a digital traffic law and order enforcement system. This system has a frontoffice application that is accessed by clients to confirm violations, check vehicle status, etc. In addition, there is a backoffice application that is accessed from the officer's side in the form of an admin dashboard to help officers manage violations.",
        screenshot: "/src/assets/etle-nasional.png",
        link: "#",
    },
    {
        name: "DeBio Network",
        description: "DeBio is the anonymous-first appchain for medical and bioinformatics services & data. In this project i worked as a UI/UX designer who designed the UI design and made a prototype using Figma.",
        screenshot: "/src/assets/debio.png",
        link: "#",
    },
    {
        name: "Intermountain West Joint Venture",
        description: "This is the company profile website of an environmental organization from USA. I built this website using WordPress.",
        screenshot: "/src/assets/iwjv.png",
        link: "#",
    },
];
</script>