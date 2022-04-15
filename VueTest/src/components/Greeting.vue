<template>
    <div class="container">
        <div class="row">
            <div class="col-md-5">
                <div class="card shadow-lg">
                    <div class="card-body">
                        <p class="h3">Hello, {{this.msg}}</p>
                        <button @click="morning('Good Morning')" class="btn btn-success btn-sm m-1">Good Morning</button>
                        <button @click="afternoon('Good Afternoon')" class="btn btn-warning btn-sm m-1">Good Afternoon</button>
                        <button @click="evening('Good Evening')" class="btn btn-danger btn-sm m-1">Good Evening</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Greeting",
    data: function(){
        return{
            msg: ""
        }
    },
    methods:{ 
        morning(value){
            this.msg = value
        },
        afternoon(value){
            this.msg = value
        },
        evening(value){
            this.msg = value
        }
    }
}
</script>

<style scoped>
</style>