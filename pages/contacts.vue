<template>
    <div class="the_container">
        <nav>
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/projects">Projects</NuxtLink>
            <NuxtLink to="/contacts">Contacts</NuxtLink>
        </nav>
        <h1>Contact Me</h1>
        <p>Fill Out Personal and Contact Details Down Below</p>
        <form name="contact" method="POST" data-netlify="true">
            <input type="hidden" name="form-name" value="contact"/>
            <label>Name: </label>
            <input type="text" name="name" required/>
            <label>Email: </label>
            <input type="email" name="email" required/>
            <label>Message: </label>
            <textarea name="message" rows="4" required></textarea>
            <button type="submit">Submit</button>
        </form>
    </div>
</template>