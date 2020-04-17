<template>
  <div class="container">
    <div class="row justify-content-center text-center py-5">
      <div class="col-12 col-md-8 col-lg-6">
        <prismic-image class="mb-3" :field="logo" width="52" />
        <h1 class="text-primary">
          {{ header }}
        </h1>
        <prismic-rich-text class="mb-0" :field="text" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Center9',
  props: {
    logo: {
      type: String,
      default: 'allo'
    },
    header: {
      type: String,
      default: 'allo'
    },
    text: {
      type: String,
      default: 'allo'
    }
  }
}
</script>
