<script setup>
import { TresCanvas } from '@tresjs/core'
import { OrbitControls, MeshGlassMaterial } from '@tresjs/cientos';
</script>


<template>
 <TresCanvas clear-color="white" window-size>
    <TresPerspectiveCamera :position="[3, 1, 3]" :look-at="[0, 0, 0]" />
    <OrbitControls />
    <TresMesh>
      <TresBoxGeometry :args="[1, 1, 1]" />
      <MeshGlassMaterial color="blue"/>
    </TresMesh>
  </TresCanvas>
</template>


<style scoped>

  *{
    margin: 0;
    padding: 0;
  }

  body, #app  {
    height: 100vh;
    width: 100%;
  }

</style>
