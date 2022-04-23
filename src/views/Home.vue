<template>
    <div>
        <h3>
            Hello from Home!
        </h3>
        <span style="display: block;">{{ count }}</span>
        <button style="display: block;" class="bg-sky-600 hover:bg-blue-800 text-white font-bold rounded py-2 px-2 my-2"
            @click="count++">Increment</button>
        <button class="bg-sky-600 hover:bg-blue-800 text-white font-bold rounded py-2 px-2"
            @click="count--">Decrement</button>
    </div>
</template>

<script>
import { ref } from "vue"
export default {
    setup() {
        const count = ref(0)
        return {
            count
        }
    },
    mounted() {
        console.log(this.count)
    }
}
</script>