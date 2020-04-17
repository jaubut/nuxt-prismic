<template>
  <div class="container">
    <div :class="['row pt-5 ', classes]">
      <div class="col-12 col-md-5">
        <h4 class="text-secondary">
          {{ tagline }}
        </h4>
        <h1 class="text-primary">
          {{ headline }}
        </h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Texts2',
  props: ['tagline', 'headline', 'classes']
}
</script>

<style>
.centercenter {
  justify-content: center;
  text-align: center;
}
</style>
