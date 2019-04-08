<template>
  <div id="home">
    <Carousel/>
  </div>
</template>

<script>
import Carousel from '@/components/Carousel';
export default {
  name: 'home',
  components: {
    Carousel
    
  }
}
</script>
<style lang="scss" scoped>
#home{
  position: relative;
  width: 100%;
}
</style>

