<script setup>
import 'x3dom'
import 'x3dom/x3dom.css'

defineProps({
  msg: String,
})

</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="container">
    <p>This is my X3D scene</p>
    <x3d width='500px' height='400px'>
      <scene>
        <shape>
          <appearance>
            <material diffuseColor='1 0 0'></material>
          </appearance>
          <box></box>
        </shape>
      </scene>
    </x3d>
  </div>
</template>

<style scoped>
/* fill for style */
</style>
