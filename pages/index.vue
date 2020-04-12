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
      logo="index.fields.center9.fields.logo.fields.file.url"
      header="index.fields.center9.fields.headline"
      text="index.fields.center9.fields.text1"
    />
    <right16
      id="apropos"
      :image="center.body[0].primary.image_banner"
      logo="index.fields.right16.fields.logo1.fields.file.url"
      :headline="$prismic.asText(center.body[0].primary.title_of_banner)"
      :text="center.body[0].primary.description"
    />
    <texts2
      id="ressource"
      tagline="index.fields.texte2.fields.tagline"
      headline="index.fields.texte2.fields.headline"
    />
    <grids5 />
    <center1
      tagline="Don"
      headline="document.data.center.headline"
      link1="https://www.paypal.com/paypalme/rejtherhotmailcom"
      linktitle="Nous soutenir via PayPal"
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
        center: homepage
      }
    } catch (e) {
      error({ statusCode: 404, message: 'Page not found' })
    }
  }
}
</script>

<style>

</style>
