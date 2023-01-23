<template>
    <pre>
        {{ this.isLoggedIn }}
    </pre>
    <div class="container">
        <div class="row">
            <div class="col-md-6">
                <div class="card">
                    <div class="card-body">
                        <div>
                            <div v-if="this.isLoggedIn" >
                                <p class="h3 fw-bold text-success">Welcome {{this.user}}</p>
                                <p> IN!! Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, soluta alias. Labore libero doloribus quisquam nisi veritatis laudantium aspernatur reprehenderit?</p>
                            </div>
                            
                            <div v-if="!this.isLoggedIn" >
                                <p class="h3 fw-bold text-danger">Thank You! {{this.user}}</p>
                                <p> OUT!! Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, soluta alias. Labore libero doloribus quisquam nisi veritatis laudantium aspernatur reprehenderit?</p>
                            </div>
                        </div>
                        <div>
                            <button v-if="!this.isLoggedIn" @click="login()" class="btn btn-success btn-sm m-1">Log In</button>
                            <button v-if="this.isLoggedIn"  @click="logOut()" class="btn btn-danger btn-sm m-1">Log Out</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'AuthUserIndex',
    data : function(){
        return {
            isLoggedIn : false
        }
    },
    methods: {
        login : function(){
            this.isLoggedIn = true
        },
        logOut : function (){
            this.isLoggedIn = false
        }
    }
}
</script>