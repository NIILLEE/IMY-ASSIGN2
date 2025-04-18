<template>
    <div class="the_card">
        <h2>A Random Animal Fact</h2>
        <p v-if="fact">{{ fact }}</p>
        <p v-else>Loading the fact...</p>
    </div>
</template>

<script setup>
    import { ref, onMounted } from 'vue';

    const fact = ref('');

    onMounted(async () => {
        const res = await fetch('https://catfact.ninja/fact');
        const data = await res.json();
        fact.value = data.fact;
    })
</script>