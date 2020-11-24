<template>
  <div class="home">
    <Header />
    <HeaderMaterial />
    <DiagonalBase :color="white" :height="conceptHeight" direction="left" top="top" bottom="bottom" id="concept">
      <Concept />
    </DiagonalBase>
    <DiagonalBase :color="pink" :height="whatHeight" direction="right" top="top" bottom="bottom" id="what">
      <What />
    </DiagonalBase>
    <DiagonalBase :color="white" :height="principlesHeight" direction="left" top="top" bottom="bottom">
      <Principles />
    </DiagonalBase>
    <Shop />
    <DiagonalBase :color="pink" :height="footerHeight" direction="left" top="top">
      <Footer />
    </DiagonalBase>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import HeaderMaterial from '@/components/HeaderMaterial.vue'
import DiagonalBase from '@/components/DiagonalBase.vue'
import Concept from '@/components/Concept.vue'
import What from '@/components/What.vue'
import Principles from '@/components/Principles.vue'
import Shop from '@/components/Shop.vue'

export default {
  name: 'Home',
  components: {
    Header,
    HeaderMaterial,
    DiagonalBase,
    Concept,
    What,
    Principles,
    Shop
  },
  data() {
    return {
      white: 'white',
      pink: '#EC376D',
      conceptHeight: '1125px',
      whatHeight: '1005px',
      principlesHeight: '2328px',
      footerHeight: '323px'
    }
  }
}
</script>

<style lang="less">

  #concept {
    color: #EC376D;
  }

  #what {
    color: white;
  }
</style>

