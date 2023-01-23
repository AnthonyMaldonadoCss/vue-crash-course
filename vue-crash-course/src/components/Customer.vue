<template>
    <div class="container">
        <div class="row">
            <!-- <p class="h3"> {{ name }} </p> -->
            <!-- <p class="h3"> {{ age }} </p> -->
            <!-- <p class="h3"> {{ designation }} </p> -->
            <!-- <input type="text"> -->
            <ul class="list-group">
                <li class="list-group-item">
                    Name: {{ name }}
                </li>
                <li class="list-group-item">
                   Age: {{ age }}
                </li>
                <li class="list-group-item">
                    Designation : {{ designation }}
                </li>
            </ul>

        </div>
    </div>
</template>

<script>
export default ({
    name: 'CustomerIndex',
    props: {
        name: {type: String, require: true},
        age : {type: Number, require: true},
        designation: {type: String, require: true},
    }
});
</script>

<style>

</style>
