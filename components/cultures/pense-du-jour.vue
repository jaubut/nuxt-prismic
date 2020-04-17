<template>
  <div class="container">
    <div class="row justify-content-between align-items-center py-5">
      <div class="col-12 col-md-5">
        <h4>{{ tagline }}</h4>
        <h1 class="display-4">
          {{ headline }}
        </h1>
        <div class="row">
          <div class="col-6">
            <i class="mb-2 fas fa-user-alt" />
            <div class="small">
              {{ feature1 }}
            </div>
          </div>
          <div class="col-6">
            <i class="mb-2 fas fa-user-friends" />
            <div class="small">
              {{ feature2 }}
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 pl-md-0 mb-4 mb-md-0">
        <div class="images-ratio ratio-4-3 w-100 mb-3" :style="'background-image: url(' + image + ')'" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cover5',
  props: {
    tagline: {
      type: String,
      default: 'tagline'
    },
    headline: {
      type: String,
      default: 'headline'
    },
    feature1: {
      type: String,
      default: 'feature1'
    },
    feature2: {
      type: String,
      default: 'feature2'
    },
    image: {
      type: String,
      default: 'image'
    }
  }
}
</script>

<style scoped>
</style>
