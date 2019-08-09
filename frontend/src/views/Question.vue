<template>
    <div class="single-question mt-2">
        <div class="container">
            {{ slug }}
        </div>
    </div>
</template>

<script>
export default {
    name: "Question",
    props: {
        slug: {
            type: String,
            required: true
        }
    }    
}
</script>

<style>

</style>
