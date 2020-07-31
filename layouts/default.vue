<template>
  <div>
    <ejm-header>
      <img slot="navigation-logo" src="~@/assets/images/sample-logo.png" alt="sample logó" />
      <li
        slot="navigation-list-item"
        class="navigation-list-item"
        v-scroll-to="'#advantages'"
      >
      <nuxt-link to='/?t=advantages'>Előnyök</nuxt-link> 
      </li>
      <li
        slot="navigation-list-item"
        class="navigation-list-item"
        v-scroll-to="'#interface'"
      >
      <nuxt-link to='/?t=interface'>Gépi interface</nuxt-link> 
      </li>
      <li
        slot="navigation-list-item"
        class="navigation-list-item"
      >
      <nuxt-link to='/?t=referenciak'>A rendszer működése</nuxt-link> 
      </li>
      <li
        slot="navigation-list-item"
        class="navigation-list-item"
      >
      <nuxt-link to='/?t=connect'>Kapcsolat</nuxt-link> 
      </li>
      <li slot="navigation-list-item" class="navigation-list-item">
        <nuxt-link to="/aloldal">Aloldal</nuxt-link>
      </li>
    </ejm-header>

    <Nuxt />

    <ejm-footer id="connect">
      <ejm-container-header slot="footer-header" class="footer-header" id="connect">
        <h2 slot="ContainerHeaderTitle">Szakértői támogatás</h2>
        <P
          slot="containerHeaderParagraph"
        >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut iaculis lobortis lorem quis sagittis. Mauris scelerisque pulvinar dolor, sit amet dapibus mi. Aenean quis fermentum magna, a placerat quam. Donec non ligula sagittis, porta metus nec, blandit quam.</P>
      </ejm-container-header>
      <img slot="footer-logo" src="~@/assets/images/sample-logo.png" alt="leiras" />
    </ejm-footer>
  </div>
</template>

<script>
export default {
  scrollToTop: true
};
</script>

<style lang="scss">
</style>
