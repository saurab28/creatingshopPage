<script setup>
import { ref } from 'vue'

const open = ref(false)
</script>

<template>
  <button @click="open = true">Open Modal</button>

  <Teleport to="body">
      <div v-if="open" class="modal">
        <p>This is a full-screen modal</p>
        <button @click="open = false">Close</button>
      </div>
    </Teleport>
</template>

<style scoped>
.modal {
  position: fixed;
  z-index: 999;
  top: 20%;
  left: 50%;
  width: 300px;
  margin-left: -150px;
}
</style>