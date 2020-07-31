<template>
  <div id="app" class="jbk">
    <client-only>

      <ejm-container-header class="navigation-header">
        <h1 slot="ContainerHeaderTitle" class="page-main-title">PAGE MAIN TITLE</h1>
        <p slot="containerHeaderParagraph">PAGE MAIN PARAGRAPH</p>
      </ejm-container-header>

      <div class="container md-column row justify-centered">
        <ejm-info-box id="advantages">
          <img
            slot="infoboxImage"
            src="~@/assets/images/sample-infobox-icon.png"
            alt="pontos leírás"
          />
          <h2 slot="infoboxTitle">Infobox Title</h2>
          <p
            slot="infoboxParagraph"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce pulvinar tincidunt auctor. Morbi non turpis maximus, finibus libero at, finibus sem.</p>
          <ejm-button
            slot="infoboxButton"
            class="button--ehk"
            href="https://www.google.hu/"
            buttonNameValue="Tovább"
          ></ejm-button>
        </ejm-info-box>

        <ejm-info-box>
          <img
            slot="infoboxImage"
            src="~@/assets/images/sample-infobox-icon.png"
            alt="pontos leírás"
          />
          <h2 slot="infoboxTitle">Infobox Title</h2>
          <p
            slot="infoboxParagraph"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce pulvinar tincidunt auctor. Morbi non turpis maximus, finibus libero at, finibus sem.</p>
          <ejm-button
            slot="infoboxButton"
            class="button--ehk"
            href="https://www.google.hu/"
            buttonNameValue="Tovább"
          ></ejm-button>
        </ejm-info-box>

        <ejm-info-box>
          <img
            slot="infoboxImage"
            src="~@/assets/images/sample-infobox-icon.png"
            alt="pontos leírás"
          />
          <h2 slot="infoboxTitle">Infobox Title</h2>
          <p
            slot="infoboxParagraph"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce pulvinar tincidunt auctor. Morbi non turpis maximus, finibus libero at, finibus sem.</p>
          <ejm-button
            slot="infoboxButton"
            class="button--ehk"
            href="https://www.google.hu/"
            buttonNameValue="Tovább"
          ></ejm-button>
        </ejm-info-box>
      </div>

    </client-only>
  </div>
</template>

<script>
export default {
   mounted() {
      setTimeout(()=> {
        this.scroll()
      }, 10)
    },
    methods: {
      scroll() {
        let el = window.location.href.split("/?t=")[1]
        let ele = document.getElementById(el)
        if(ele)
          this.$scrollTo(ele, 1000)
      }
    }
};
</script>

<style lang="scss">
@import "~@/assets/styles/fonts.css";
h1,
h2 {
  font-family: PlayFairDisplay;
}
p,
span {
  font-family: SourceSansPro;
}
.container-header.navigation-header {
  background-image: url("~@/assets/images/sample-header-image.png");
}
</style>
