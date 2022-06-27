<template>
  <div class="col-lg-3 col-md-4 d-flex justify-content-between flex-column">
    <div class="card mt-3 card-benefit" v-for="(benefit, i) in benefits" :key="i">
      <div class="card-body d-flex align-items-center">
        <img class="me-3" :src="benefit.src" alt="icon láser">
        <p>{{benefit.text}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['benefits']
}
</script>
