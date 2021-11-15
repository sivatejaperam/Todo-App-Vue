<template>
    <button :style="{'background-color': color }" class="btn" @click="addTask">
        {{text}}
    </button>
</template>

<script>
    export default {
        name : "Button",
        props:{
            text: String,
            color: String
        },
        methods:{
            addTask() {
                this.$emit('btn-click');
            }
        }
    }
</script>