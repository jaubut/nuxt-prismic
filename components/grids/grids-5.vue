<template>
  <div class="container">
    <div class="row py-5">
      <div v-for="item in items" :key="item.index" class="col-12 col-md-3 mb-4 mb-md-0">
        <h4 class="text-secondary">
          {{ $prismic.asText(item.headline) }}
        </h4>
        <prismic-rich-text class="small" :field="item.richtext" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Grids5',
  props: {
    items: {
      type: Array,
      default () {
        return []
      }
    }
  }
}
</script>
