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
    <x3d width='466px' height='233px' showStat="true">
      <scene>
        <viewpoint description="Entry" position="0 1 -3.5" orientation="0 1 0 3.14" />
        <inline mapDEFToID="true" url="Deer.x3d">
        </inline>
      </scene>
    </x3d>
  </div>

</template>

<style scoped>
/* fill for style */
</style>
