
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

    <Counter/>
    <br>
    <Greeting/>

    </div>
  </main>
</template>

<script>
import Counter from './components/Counter.vue'
import Greeting from './components/Greeting.vue'

  export default {
    components: {
      Counter , Greeting
    }
  }
</script>

<style>
 @import url(./assets/base.css);
</style>
