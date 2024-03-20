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
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui quibusdam consequatur expedita molestiae quidem, fugit minus maxime necessitatibus deserunt quaerat sunt? Doloremque, quisquam. Quisquam cupiditate nulla vero, nihil dignissimos ex exercitationem ducimus odio.</p>
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
<style>
p{
  color: sandybrown;
}
</style>