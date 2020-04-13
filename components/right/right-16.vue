<template>
  <div class="container">
    <div class="row justify-content-between align-items-center py-5">
      <div class="col-12 col-md-6 pl-md-0 mb-4 mb-md-0">
        <prismic-image class="w-100" :field="image" />
      </div>
      <div class="col-12 col-md-5">
        <prismic-image class="mb-3" :field="logo" width="40" />
        <h3 class="display-4 text-primary">
          {{ headline }}
        </h3>
        <prismic-rich-text class="small" :field="text" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Right16',
  props: ['image', 'logo', 'headline', 'text']
}
</script>
