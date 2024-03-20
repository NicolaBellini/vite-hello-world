<script>
export default {
  data() {
    return {
      title:'Hello word!',
      isHovered:false
    }
  },
  methods: {

  },
}
</script>

<template>

<div
    :class="{'hovered':isHovered}"
    class="container"
    @mouseenter="isHovered=true"
    @mouseleave="isHovered=false">
    <h1 class="mt-2">{{ title }}</h1>
  </div>

</template>

<style scoped>
.container{
  background-color: red;
}
.hovered{
background-color: blue;
}
</style>