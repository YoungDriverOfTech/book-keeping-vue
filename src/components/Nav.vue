<template>
    <nav class="nav">
        <router-link to="/money" class="item" active-class="selected">
            <Icon name="money"/>
            记账
        </router-link>
        <router-link to="/labels" class="item" active-class="selected">
            <Icon name="labels"/>
            标签
        </router-link>
        <router-link to="/statistics" class="item" active-class="selected">
            <Icon name="statistics"/>
            统计
        </router-link>
    </nav>
</template>

<script lang="ts">
    export default {
        name: 'Nav'
    };
</script>

<style lang="scss" scoped>
    @import "~@/assets/style/helper.scss";
    /* scoped 表示这个class的作用域只能在此div里面起作用*/
    .nav {
        display: flex;
        flex-direction: row;
        font-size: 12px;
        @extend %outerShadow;
        > .item {
            padding: 2px 0;
            width: 33.333333%;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        .icon{
            width: 32px;
            height: 32px;
        }
        > .item.selected{
            font-weight: bold;
            color: dodgerblue;
        }
    }
</style>