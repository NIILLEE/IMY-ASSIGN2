<template>
    <div class="center_container">
        <img src="../assets/profile.jpg" alt="Profile Photo" width="500" class="profile"/>
        <h1>Shariff Muhammad</h1>
        <p>I am an aspiring Software Developer who is passionate about being creative with code and everything else, allowing people to see the world in a unique perspective.</p>
        <Weather/>
        <FactsAnimal/>
    </div>
</template>

<script>
import FactsAnimal from '~/components/FactsAnimal.vue';
import Weather from '~/components/Weather.vue';
</script>