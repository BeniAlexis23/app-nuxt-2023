<script stup lang="ts">
    definePageMeta({
        layout: 'authentication'
    })
</script>

<template>
<div class="container">
    <div class="row">
        <h1>My Account</h1>
    </div>
    <div class="row">
        <div class="col-6">
            <nuxt-link class="btn btn-primary" to="/account">Login</nuxt-link>
            <nuxt-link class="btn btn-primary" to="/account/register">Register</nuxt-link>
        </div>
        <div class="col-6">
            <NuxtPage/>
        </div>
    </div>
</div>
</template>