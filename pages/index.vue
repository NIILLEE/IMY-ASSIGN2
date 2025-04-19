<template>
    <div class="center_container">
        <nav>
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/projects">Projects</NuxtLink>
            <NuxtLink to="/contacts">Contacts</NuxtLink>
        </nav>
        <img src="../assets/profile.jpg" alt="Profile Photo" width="500" class="profile"/>
        <h1>Shariff Muhammad</h1>
        <h2>Welcome To My PORTFOLIO!</h2>
        <p>I am an aspiring Software Developer who is passionate about being creative with code and everything else, allowing people to see the world in a unique perspective.</p>
        <Weather/>
        <FactsAnimal/>
    </div>
</template>

<script>
import { NuxtLink } from '#components';
import FactsAnimal from '~/components/FactsAnimal.vue';
import Weather from '~/components/Weather.vue';
</script>