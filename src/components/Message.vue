<template>
    <div class="message-container" v-if="teste">
        <p>{{ msg }}</p>
    </div>
    <div class="message-container-f" v-else>
        <p>{{ msg }}</p>
    </div>
</template>

<script>
export default {
    name: 'Message',
    props: {
        msg: String,
        teste: Boolean
    }
}
</script>

<style scoped>
    .message-container {
        color: #004085;
        background-color: #CCE5FF;
        border: 2px solid #B8DAFF;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }
    .message-container-f {
        color: #850000;
        background-color: #ffcccc;
        border: 2px solid #ffb8b8;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }
</style>