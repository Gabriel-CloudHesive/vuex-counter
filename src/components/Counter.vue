<template>
    <div>
        <button @click="increment(2)"> Increment</button >
            <div>
                {{ counter }}
            </div>
            <button @click="decrement(3)">Decrement</button>
    </div>
</template>

<script>
import { mapState, mapMutations } from "vuex";
    export default {
        computed: {
            ...mapState(['counter'])
        },
        methods: {
            ...mapMutations(['increment', 'decrement'])
        }
    }
</script>