<template>
    <p class="text">
        <slot></slot>
    </p>
</template>
<script>
export default {
    name: 'my-text'
}
</script>
<style scoped>
.text {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;
}
</style>