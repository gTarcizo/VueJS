<template>
<session>
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <div class="card" >
                        <div class="card-body">
                            <div v-if="isLogged">
                                <p class="h3 fw-bold text-success">Welcome User</p>
                                <p class="fst-italic">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed eaque pariatur consequuntur voluptates voluptas quo, harum sunt laudantium tempora maxime ex laboriosam aspernatur aliquam. Totam officia rerum earum dolorum neque!</p>
                            </div>
                        </div>
                        <div class="card-body">
                            <div v-if="!isLogged">
                                <p class="h3 fw-bold text-warning">Now You Are Not Logged</p>
                                <p class="fst-italic">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iure minus nesciunt ut animi unde, praesentium mollitia blanditiis, fugit cum modi velit aliquam, facere vero. Obcaecati iste fugiat quaerat officiis eveniet.</p>
                            </div>
                        </div>
                        <div>
                            <button class="btn btn-success btn-sm m-3" @click="login()"> Login</button>
                            <button class="btn btn-warning btn-sm m-3 text-white" @click="logout()"> Logout</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</session>
</template>
<script>
export default {
    name: 'AuthUser',
    data(){
    return{
        isLogged: false
    }

    },
    methods:{
        login(){
            this.isLogged = true
        },
        logout(){
            this.isLogged = false
        }
        
}
}
</script>