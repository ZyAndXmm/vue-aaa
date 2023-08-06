<template>
    <div>
        <h1>
            父组件
        </h1>
        <br>
        <commonChild :msg="msg" :obj="obj" :arr="arr"/>
    </div>
</template>

<script>
import commonChild from '@/views/commonChild.vue'
    export default {
        data () {
            return {
                msg: '我是子组件的数据',
                obj: {
                    a: 1,
                    b: 2
                },
                arr:[1,2,3]
            }
        },
        components: {
            commonChild
        }
    }
</script>

<style lang="scss" scoped>

</style>