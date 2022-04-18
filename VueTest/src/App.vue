
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
  <UserList/>

  </div>
  </main>
</template>

<script>
import UserList from './components/UserList.vue'
import Spinner from './components/Spinner.vue'

  export default {
    components: { UserList , Spinner}
}
</script>

<style>
 @import url(./assets/base.css);
</style>
