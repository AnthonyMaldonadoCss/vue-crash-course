<template>
    <div class="container mt-3">
        <div class="grid">
            <div class="row">
                <div class="col">
                    <h3 class="h3 text-success fw-bold">App component</h3>
                    <p class="fst-italic">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad facere quam nesciunt quibusdam enim praesentium ipsa fugiat placeat maiores deserunt vero totam, laborum nemo hic odit quo aliquam quisquam dolorem!</p>

                </div>
            </div>
        </div>
        <!-- <CustomerIndex name="Anthony" age="27" designation="Software Enginner"/> -->
        <!-- <CustomerIndex name="Heczaid" age="27" designation="Bioanalista" /> -->
        <!-- <CustomerIndex/> -->
        <!-- <CustomerIndex/> -->
        <!-- <EmployeeIndex/> -->
        <!-- <CounterIndex/> -->
        <!-- <GreetingsIndex/> -->
        <!-- <RegisterIndex/> -->
        <!-- <AuthUserIndex/> -->
        <ListRenderingIndex/>
    </div>
</template>

<script>
// import CounterIndex from './components/Counter.vue'
// import GreetingsIndex from './components/Greeting.vue'
// import CustomerIndex from '@/components/Customer.vue'
// import EmployeeIndex from './components/Employee.vue'
// import RegisterIndex from './components/Register.vue'
// import AuthUserIndex from './components/AuthUser.vue'
import ListRenderingIndex from './components/listRendering.vue'
export default {
  name: 'App',
  components: {ListRenderingIndex}
}
</script>

<style>
@import "./views/styles.css";
</style>