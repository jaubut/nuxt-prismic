<template>
  <div>
    <div class="bg-cover chantal-cover text-white" :style="'background-image:url(' + index.body[0].primary.background_image.url + ');'">
      <menu4 />
      <culture1
        :tagline="index.body[0].primary.tagline"
        :headline="index.body[0].primary.headline"
        :text="index.body[0].primary.rich_text"
        link-text="index.fields.culture1.fields.link1"
        cta="S’inscrire"
      />
    </div>
    <center9
      :logo="index.body[1].items[0].logo"
      :header="index.body[1].primary.headline"
      :text="index.body[1].primary.rich_text"
    />
    <right16
      id="apropos"
      :image="index.body[2].items[0].image"
      :logo="index.body[1].items[0].logo"
      :headline="index.body[2].primary.headline"
      :text="index.body[2].primary.rich_text"
    />
    <texts2
      id="ressource"
      :tagline="index.body[3].primary.tagline"
      :headline="$prismic.asText(index.body[3].primary.headline)"
    />
    <grids5
      :items="index.body[4].items"
    />
    <center1
      :tagline="index5.primary.tagline"
      :headline="index5.primary.headline"
      :link1="index5.primary.link1"
      :linktitle="index5.primary.link1_label"
    />
    <div>
      <audio controls>
        <source src="https://soundcloud.com/pensee-du-jour/ps-91-v-14" type="audio/mpeg">
      Your browser does not support the audio element.
      </audio>
    </div>
    <footers8 />
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
        index: homepage,
        index5: homepage.body[5]
      }
    } catch (e) {
      error({ statusCode: 404, message: 'Page not found' })
    }
  }
}
</script>

<style>
.chantal-cover {
  background-color: black;
  background-position: center center;
  background-size: cover;
  min-height: 70vh;
}
</style>
