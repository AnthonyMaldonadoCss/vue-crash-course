<template>
    <div class="container">
        <div class="row">
            <div class="col">
                <div class="h3 fw-bold text-success">User List</div>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, officia.</p>
            </div>
            <div class="row">
                <div class="col">
                    <table class="table table-hover text-center table-striped">
                        <thead class="bg-light">
                            <tr>
                                <th>#</th>
                                <th>Name</th>
                                <th>Username</th>
                                <th>Email</th>
                                <th>Address</th>
                                <th>Phone</th>
                                <th>Website</th>
                                <th>Companies</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr v-for="user in this.users" :key="user.id" >
                            <td>{{ user.id }}</td>
                            <td>{{ user.name }}</td>
                            <td>{{ user.username }}</td>
                            <td>{{ user.email }}</td>
                            <td>{{ user.address.street }}</td>
                            <td>{{ user.phone }}</td>
                            <td>{{ user.website }}</td>
                            <td>{{ user.company.name}}</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { UserService } from '@/services/userServices';
export default {
    name : 'ListRenderingIndex',
    data : function(){
        return {
            users : UserService.getAllUsers()
        }
    }
}
</script>