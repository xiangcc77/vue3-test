<script setup>
// 1.reactive 接收一个对象类型的数据，返回一个响应式的对象
// import {reactive} from 'vue'
// const state = reactive({count: 100})

// const addOne = () => {
//     state.count++
// }

// 2.ref 接收简单类型 或 复杂类型，返回一个响应式对象
import {ref} from 'vue'
const state = ref(100)

const addOne = () => {
    console.log(state.value)
    state.value++
}
</script>

<template>
    <div>
        <div>{{ state }}</div>
        <button @click="addOne">+1</button>
    </div>
</template>

<style scoped></style>