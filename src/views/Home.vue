<template>
    <div>
        <h3>
            Hello from Home!
        </h3>
        <span style="display: block;">{{ count }}</span>
        <button @click="count++">Increment</button>
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