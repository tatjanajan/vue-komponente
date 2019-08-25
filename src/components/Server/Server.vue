<template>
    <li class="list-group-item" @click="serverSelected">Server #{{ server.id }}</li>
</template>
<script>

import { serverBus } from '../../main.js'

export default {
    props: ['server'],
    methods: {
        serverSelected() {
            serverBus.$emit('serverSelected', this.server)
        }
    }
}
</script>

<style scoped>
    li {
        cursor: pointer;
    }

    li:hover {
        background-color: #e9e9e9;
    }
</style>