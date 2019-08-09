<template>
    <div>
        <h1>{{ message }}</h1>
        <button v-on:click="reverseMessage">Перевернуть сообщение</button>
        <h1>{{kek}}</h1>
    </div>
</template>

<script>

    export default {
        props:[
            "kek"
        ],
        data: function(){
            return {
                message: "1_2_3_4_5_6_7_8_9_0"
            }
        },
        methods: {
            reverseMessage: function () {
                this.message = this.message.split('').reverse().join('');
                console.log(this.kek)
            }
        }

    }
</script>

<style scoped>

</style>
