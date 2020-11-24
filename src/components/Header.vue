<template>
    <header id="header">
        <h1 class="header-logo"><img :src="image_src" alt="" class="header-logo-img"></h1>
    </header>
</template>

<script>
export default {
    data () {
        return {
            image_src: require('@/assets/header_logo.png')
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
    .header-logo {
        position: absolute;
        z-index: 1;
        right: 50%;
        transform: translate(50%);
    }
</style>
