<template>
    <div class="nav">
        <router-link to="/money">记账</router-link>
        |
        <router-link to="/labels">标签</router-link>
        |
        <router-link to="/statistics">统计</router-link>
    </div>
</template>

<script lang="ts">
    export default {
        name: "Nav"
    }
</script>

<style lang="scss" scoped>
    /* scoped 表示这个class的作用域只能在此div里面起作用*/
    .nav{
        border: 1px solid red;
    }
</style>