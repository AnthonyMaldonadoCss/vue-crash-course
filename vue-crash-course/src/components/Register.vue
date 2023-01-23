<template>
    <pre>{{ this.user }}</pre>
    <div class="containter">
        <h2>Register</h2>
        <div class="row">
            <div class="col-md-3">
                <div class="card shadow-lg">
                    <div class="card-header bg-success text-white">
                        <p class="h3">Register Here</p>
                    </div>
                    <div class="card-body  bg-light">
                        <form @submit.prevent="register()">
                            <div class="mb-2">
                                <div class="mb-2">
                                    <input v-model="user.name" required autocomplete="false" onfocus type="text" placeholder="Name" class="form-control">
                                </div>
                                <div class="mb-2">
                                    <input v-model="user.password" required autocomplete="false" type="password" placeholder="password" class="form-control">
                                </div>
                                <div class="mb-2">
                                    <input v-model="user.email" required autocomplete="false" type="email" placeholder="Email" class="form-control">
                                </div>
                                <div class="mb">
                                    <input type="submit" placeholder="Register" class="form-control">
                                </div>
                            </div>
                        </form>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'RegisterIndex',
    data : function(){
        return {
            user :{
                name: '',
                email: '',
                password: '' 
            }
        }
    },
    methods:{
        register: function(){
            console.log(this.user)
        }
    }

}
</script>