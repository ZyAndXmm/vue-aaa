<template>
    <div>
        子组件
        {{ msg }}
        {{ a }}
        <ul>
            <li v-for="item in arr">
                {{ item }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: {
            msg: String,
            a:{
                type: String,
                default: '我是默认数据'
            },
            arr: {
                type: Array,
                default: [4,5,6]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>