<template>
<section>
  <MobileToolBar v-if="$vuetify.breakpoint.xsOnly" />
  <LaptopToolBar v-else />
</section>
</template>

<script>
import MobileToolBar from './MobileToolBar'
import LaptopToolBar from './LaptopToolBar'

export default {
  name: 'ToolBar',
  components: { MobileToolBar, LaptopToolBar },
  props: {},
  data() { return {} },
  mounted() {},
  computed: {},
  methods: {}
}
</script>

<!-- Add 'scoped' attribute to limit CSS to this component only -->
<style lang="sass" scoped>
// .border
//     border: 1px dashed grey
</style>
