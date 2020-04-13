<template>
  <div>
    <div class="bg-cover chantal-cover text-white">
      <menu4 />
      <culture1
        tagline="index.fields.culture1.fields.tagline"
        headline="index.fields.culture1.fields.headline"
        text="index.fields.culture1.fields.text"
        link-text="index.fields.culture1.fields.link1"
        cta="S’inscrire"
      />
    </div>
    <center9
      :logo="index.body[1].items[0].logo.url"
      :header="index.body[1].primary.headline"
      :text="$prismic.asText(index.body[1].primary.rich_text)"
    />
    <!--<right16
      id="apropos"
      image="index.body[2].items[0].image.url"
      logo="index.body[1].items[0].logo.url"
      :headline="$prismic.asText(index.body[2].primary.headline)"
      :text="$prismic.asText(index.body[2].primary.rich_text)"
    />-->
    <texts2
      id="ressource"
      :tagline="index.body[3].primary.tagline"
      :headline="$prismic.asText(index.body[3].primary.headline)"
    />
    <grids5
      :items="index.body[4].items"
    />
    <center1
      :tagline="$prismic.asText(index.body[5].primary.tagline)"
      :headline="$prismic.asText(index.body[5].primary.headline)"
      :link1="index.body[5].primary.link1"
      :linktitle="$prismic.asText(index.body[5].primary.link1_label)"
    />
  </div>
</template>

<script>

export default {
  components: {
  },
  async asyncData ({ $prismic, error }) {
    try {
      // Query to get the home page content
      const homepage = (await $prismic.api.getSingle('accueil')).data

      return {
        // Page content
        index: homepage
      }
    } catch (e) {
      error({ statusCode: 404, message: 'Page not found' })
    }
  }
}
</script>

<style>

</style>
