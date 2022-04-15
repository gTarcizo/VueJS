<!-- Todo componente tem que estar com a Letra maiúscula -->
<template>
    <div class="container shadow-lg">
        <div class="row">
            <div class="col-mds-4">
                <div class="card">
                    <div class="card-header">
                        <div class="card-body">
                            <p class="h3 display-3 text-center">{{this.count}}</p>
                            <button v-on:click="increment" class="btn btn-success m-1">Increment</button> <!-- v-on:click="" Ou @click="function()" -->
                            <button @click="decrement()" class="btn btn-warning m-1">Decrement</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function(){ // você tem que declarar um state
        return{
            count : 0
        }
    },
    methods: {
    increment(){
        this.count++
    },
    decrement(){
        this.count--
    }
    }
}
</script>

<style scoped>

</style>