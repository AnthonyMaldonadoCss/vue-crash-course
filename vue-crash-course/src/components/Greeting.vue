<template>
    <div class="container">
        <div class="row">
            <div class="col-md-6">
            <div class="card shadow-lg">
                <div class="card-body">
                    <p class="h3">
                        Hello <span class="fw-bold">{{ this.msg }}</span> 
                    </p>
                    <button class="btn btn-success m-1" @click="greet('Good Morning')">Good Morning</button>
                    <button class="btn btn-warning m-1" @click="greet('Good Afertnoon')">Good Afternoon</button>
                    <button class="btn btn-danger m-1" @click="greet('Good Evening')">Good Evening</button>
                </div>
            </div> 
            </div>
        </div>
    </div>
</template>

<script>
export default ({
    name: 'GreetingsIndex',
    data : function(){
        return {
            msg : ''
        }
    },
    methods :{
        greet : function(value){
            this.msg = value;
        }
    }
})
</script>