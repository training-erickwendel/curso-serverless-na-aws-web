<template>
  <section class="section Sponsor">
    <div class="container SponsorContainer">
      <StyledTitle margin="0px 0px 60px 0px">Patrocinadores</StyledTitle>
      <div>
        <a
          target="_blank"
          href="https://www.facebook.com/page.erickwendel">
          <img
            src="../assets/ew-logo.png"
            alt="ew.it">
        </a>
         
        <a
          target="_blank"
          href="#">
          <img
            :style="{
              width: '130px'
            }"
            src="../assets/amigu.png"
            alt="projeto amigu">
        </a>
        <a
          target="_blank"
          href="https://www.facebook.com/gruporesolvdata/">
          <img
            src="../assets/resolv.png"
            alt="grupo resolv">
        </a>
        
      </div>
    </div>
  </section>
</template>

<script>
import StyledTitle from './Title';

export default {
  name: 'Sponsor',
  components: { StyledTitle },
};
</script>

<style lang="scss" scoped>
.Sponsor {
  > .SponsorContainer {
    display: flex;
    flex-direction: column;
    align-items: center;

    > div {
      display: flex;
      flex-wrap: wrap;
      flex-direction: row;
      align-items: center;

      @media screen and (max-width: 700px) {
        flex-direction: column;
      }

      > a {
        @media screen and (max-width: 700px) {
          margin-top: 20px;
        }

        > img {
          display: inline-block;
          vertical-align: middle;
          max-width: 90%;
          width: 200px;
          height: auto;
          margin: 0 12px 20px 12px;
        }
      }
    }
  }
}
</style>

