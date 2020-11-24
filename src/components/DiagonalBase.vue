<template>
    <section :class="['Item' , direction, top , bottom]" :style="styles">
        <slot />
    </section>
</template>

<script>
export default {
    props: {
        color: String,
        top: String,
        bottom: String,
        height: String,
        direction: String,
    },
    computed: {
        styles () {
            return {
                '--color': this.color,
                '--height': this.height
            }
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
    .Item {
        display: block;
        width: 100%;
        position: relative;
        --color: #ccc;
        --height: 500px;
        height: var(--height);
        background-color: var(--color);
        &::before {
            content: "";
            position: absolute;
            top: -180px;
            left: 0;
            width: 0;
            height: 0;
            display: block;
        }
        &::after {
            content: "";
            position: absolute;
            bottom: -180px;
            left: 0;
            width: 0;
            height: 0;
            display: block;
        }
        &.right {
            &.top {
                &::before {
                    border-style: solid;
                    border-width: 180px 0 0 100vw;
                    border-color: transparent transparent transparent var(--color);
                }
            }
            &.bottom {
                &::after {
                    border-style: solid;
                    border-width: 180px 100vw 0 0;
                    border-color: var(--color) transparent transparent transparent;
                }
            }
        }
        &.left {
            &.top {
                &::before {
                    border-style: solid;
                    border-width: 180px 100vw 0 0;
                    border-color: transparent var(--color) transparent transparent;
                }
            }
            &.bottom {
                &::after {
                    border-style: solid;
                    border-width: 0 100vw 180px 0;
                    border-color: transparent var(--color) transparent transparent;
                }
            }
        }
    }
</style>