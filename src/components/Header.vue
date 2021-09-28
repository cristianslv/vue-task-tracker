<template>
    <header>
        <h1>{{ title }}</h1>
    </header>
    <Button text="Add Task" color="green" />
    <!-- <Button text="Update Task" color="blue" />
    <Button text="Delete Task" color="red" /> -->
</template>

<script>
import Button from "./Button";

export default {
    name: 'Header',
    props: {
        title: {
            default: "Hello World",
            required: true,
            type: String,
        }
    },
    components: {
        Button
    }
}
</script>

<style scoped>
    header {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
        justify-content: space-between;
    }
</style>
