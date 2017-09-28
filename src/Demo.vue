<template>
    <el-dialog :visible.sync="dialogFormVisible">
        <div>
            <el-button @click="changeState">关闭</el-button>
        </div>
    </el-dialog>
</template>
<script>
    export default {
        props: ['dialogFormVisible'],
        data() {
            return {
                dialogState: false
            }
        },
        methods: {
            changeState() {
                this.$emit('update:dialogFormVisible', !this.dialogFormVisible)
            }
        },
        mounted() {
            this.dialogState = this.dialogFormVisible
        }
    }
</script>
