<template>
  <div class="sponsor-list">
    <a :href="spr.href" v-for="spr in sponsorList" :target="spr.target">
      <img :alt="spr.alt" :src="spr.src" class="sponsor-item" />
    </a>
  </div>
</template>

<script>
export default {
  data () {
    return {
      sponsorList: [
        {
          alt: 'MitSport',
          href: 'https://mitsport-shop.com/creualta/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/mitsport.jpg',
          target: '_blank'
        },
        {
          alt: 'CJB',
          href: 'https://www.penya.com/ca/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/penya.gif',
          target: '_blank'
        },
        {
          alt: 'Superwagen',
          href: 'https://www.superwagen.com/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/superwagen.png',
          target: '_blank'
        },
        {
          alt: 'Infoserveis',
          href: 'https://www.infoserveis.cat/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/infoserveis.png',
          target: '_blank'
        },
        {
          alt: 'Expofinques',
          href: 'http://www.expofinques.com/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/expofinques.png',
          target: '_blank'
        },
        {
          alt: 'Ars',
          href: 'https://arssalutesportiva.com/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/ars.png',
          target: '_blank'
        },
        {
          alt: 'Agnes',
          href: '#',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/agnes.png',
          target: ''
        },
        {
          alt: 'Contrast',
          href: 'http://www.contrastrestaurant.cat/',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/contrast_200x80.png',
          target: '_blank'
        },
        {
          alt: 'Assessors March',
          href: '#',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/march2.png',
          target: ''
        },
        {
          alt: 'Winzule',
          href: '#',
          src: 'http://www.creualtabasquet.cat/patrocinadors/images/winzule.png',
          target: ''
        }
      ]
    }
  }
}
</script>

<style scoped>
.sponsor-list {
  /* background: #5575dd; */
  width: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}

.sponsor-item {
  display: block;
  max-width: 200px;
  max-height: 80px;
  width: auto;
  height: auto;
  margin: 0.5rem;
}
</style>
