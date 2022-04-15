
<template>
<main>
  <div class="container mt-3">
    <div class="grid">
      <div class="row">
        <div class="row">
          <p class="h3 text-success fw-bold">App Component</p>
          <p class="fst-italic">Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem repellat saepe in est eos eius quibusdam, amet, quidem tempora aperiam mollitia labore molestias nobis laboriosam accusantium excepturi non porro odio.</p>
        </div>
      </div>
    </div>
    
    <Customer name="Tarcizo" age="22" designation="Software Engineer" />  <!-- Carregar o componente -->
    <Employee/>
  </div>
  </main>
</template>

<script>
import Customer from './components/Customer.vue'
import Employee from './components/Employee.vue'
  export default {
    components: { Customer , Employee }
}
</script>

<style>
 @import url(./assets/base.css);
</style>
