<template>
    <article>
        <h3>{{ post.title }}</h3>
        <p>{{ post.body }}</p>
    </article>
</template>

<script>
export default {
    // name: "PostVue", 
    props: ["post"]
}
</script>

<style>

</style>