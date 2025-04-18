<template>
    <div class="the_card">
        <h2>Weather in Pretoria</h2>
        <p v-if="the_weather">{{ the_weather.main.temp }}°C - {{ the_weather.weather[0].description }}</p>
        <p v-else>Loading the weather...</p>
    </div>
</template>

<script setup>
    import { ref, onMounted } from 'vue';

    const the_weather = ref(null);

    onMounted(async() => {
        const res = await fetch(
            'https://api.openweathermap.org/data/2.5/weather?q=Pretoria&units=metric&appid=a2702b61f2b8b41615f30884700bc140'
        )
        the_weather.value = await res.json();
    })
</script>