<template>
<session>
 <!--   <pre> {{this.user}}</pre>  vai mostrar na tela o estado do meu "data()" -->
    <div class="container shadow-lg">
        <div class="row ">
            <div class="col-md-3 shadow-">
                <div class="card">
                    <div class="bg-success card-header">
                        <p class="text-white font-weight-light display-6 m-1">Register Here</p>
                    </div>
                    <div class="card-body bg-light">
                        <form @submit.prevent="register()">
                            <div class="mb-2">
                                <input v-model="user.name" type="text" class="form-control" placeholder="Name">
                            </div>
                            <div class="mb-2">
                                <input v-model="user.password" type="password" class="form-control" placeholder="Password">
                            </div>
                            <div class="mb-2">
                                <input v-model="user.email" type="email" class="form-control" placeholder="E-mail">
                            </div>
                            <div class="mb-2">
                                <input id="submitButton" type="submit" class="form-control btn-success" value="Register">
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</session>
</template>

<script>
export default {
    name: "Register",
    data(){
        return{
            user : {
                name: "",
                password: "",
                email: ""
            }
        }
    },
    methods:{
        register(){
            console.log(this.user)
        }
    }

}
</script>
