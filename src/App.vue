<template>
    <div id="app">
        <span @click="dialogFormVisible = true">点击出现弹窗</span>
        
        <demo :dialogFormVisible.sync="dialogFormVisible"></demo>
    </div>
</template>

<script>
import Demo from './Demo.vue'
export default {
    name: 'app',
    data() {
        return {
            dialogFormVisible: false
        }
    },
    components: {
        Demo
    }
}
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}

h1,
h2 {
    font-weight: normal;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
