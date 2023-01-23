<template>
    <div class="container">
        <div class="row">
            <div class="col-md-4">
                <div class="card shadow-lg">
                    <div class="card-body">
                        <p class="h3 display-3">{{this.count}}</p>
                        <button @click="incre" class="btn btn-success m-1">Incremet</button>
                        <button @click="decre" class="btn btn-warning">Decrement</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>

export default ({
    name: 'CounterIndex',
    data : function(){
        return {
            count : 0
        }
    },
    methods: {
        incre : function(){
            this.count += 1;
        },
        decre : function(){
            this.count -= 1;
        }
    }
})
</script>
