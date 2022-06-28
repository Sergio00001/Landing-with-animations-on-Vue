<template>
    <button class="btn">
        <slot></slot>
    </button>
</template>
<script>
export default {
    name: 'my-button'
}
</script>
<style scoped>
.btn {
    font-family: 'Aileron';
    border: 1px solid #FFFFFF;
    border-radius: 30px;
    padding: 3px 10px;
    background-color: #ffffff00;
    color: #FFFFFF;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    cursor: pointer;
    transition: all 0.5s ease 0s;
}

.btn:hover {
    color: black;
    background-color: #FFFFFF;
    padding: 5px 15px;
}
</style>