<template>
    <div class="app-body" id="app">
        <!--router-view-->
        <router-view>
        </router-view>
    </div>
</template>

<script>
    export default {
        name: 'app',
        components: {},
        method: {},
        ready: function () {
            console.log("APP is ready");
        },
        created: function () {
            console.log("APP is created");
            this.$router.push('/login');
        },
        mounted: function () {
            console.log("APP is mounted");
        }
    }
</script>

<style lang='less' scoped>
    .app-body {
        width: 100%;
        height: 100%;
        padding-top: 0px;
        padding-bottom: 0px;
    }
</style>
