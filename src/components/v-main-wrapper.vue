<template>
  <div class="v-main-wrapper">
    <p>{{title}}
    </p>
    <v-catolog />
    <v-cart />
  </div>
</template>

<script>

import vCatolog  from './v-catolog'
import vCart from './v-cart'

export default {
  name: 'v-main-wrapper',
  components: {
    vCatolog,
    vCart

  },
  props: {},
  data() {
    return {
      title: 'Main wrapper'
    }
  },
  computed: {

  },
  methods: {},
  watch: {},
  mounted() {
    console.log('Hello i am alive')
  }


}
</script>


<style scoped>
.v-main-wrapper{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  max-width: 900px;
  margin: 0 auto;

}
</style>