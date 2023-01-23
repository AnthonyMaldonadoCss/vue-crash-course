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
        <EmployeeIndex/>
    </div>
</template>

<script>
// import CustomerIndex from '@/components/Customer.vue'
import EmployeeIndex from './components/Employee.vue'
export default {
  name: 'App',
  components: {
    // CustomerIndex,
    EmployeeIndex
  }
}
</script>

<style>
@import "./views/styles.css";
</style>