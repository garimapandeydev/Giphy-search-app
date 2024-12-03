<template>
  <div id="gifList">
    <gif v-for="gif in gifs" :gif="gif" :key="gif.id"/>
  </div>
</template>

<script>
import Gif from "@/components/Gif";
export default {
name: "GifList",
  components: {Gif},
  props: ['gifs']
}
</script>

<style scoped>
 
#gifList {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 20px;
}

.gif {
  width: 240px;
  height: 240px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  border-radius: 8px;
}
</style>

