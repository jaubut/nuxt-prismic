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
    <pensedujour />
    <texts2
      id="ressource"
      classes="centercenter"
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
    <div class="fix-bottom">
      <iframe
        id="sc-widget"
        src="https://w.soundcloud.com/player/?url=https://api.soundcloud.com/users/157602472"
        width="100%"
        height="164"
        scrolling="no"
        frameborder="no"
      />
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
.fix-bottom {
  bottom: 0;
  width: 100vw;
  position: fixed;
  z-index: 99999;
}
</style>
