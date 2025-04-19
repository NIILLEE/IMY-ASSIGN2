<template>
    <div class="the_containers">
        <nav>
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/projects">Projects</NuxtLink>
            <NuxtLink to="/contacts">Contacts</NuxtLink>
        </nav>
        <h1>My Projects</h1>
        <div v-for="(project, index) in projects" :key="index" class="the_class">
            <h2>{{ project.name }}</h2>
            <p>{{ project.description }}</p>
        </div>
    </div>
</template>

<script setup>
    const projects = [
        { name: 'Weather', description: 'Shows live weather using OpenWeatherMap API.' },
        { name: 'To-Do List', description: 'Simple task Manager built using Vue.' },
        { name: 'Portfolio Site', description: 'This is my current website showcasing my own work.'}
    ]
</script>