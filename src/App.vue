<template>
  <q-layout view="hHh lpR fFf" class="app-layout">
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-toolbar-title>
          Tugas 1-7 Praktikum PBK
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container class="page-container">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
.app-layout {
  min-height: 100vh;
  background-image: url('../src/assets/Porche.png');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  display: flex;
  flex-direction: row-reverse; 
  font-family: 'Times New Roman', Times, serif; 
}

.page-container {
  flex-grow: 1;
  display: flex;
  justify-content: flex-start;
}

.bg-primary {
  background-color: #1976d2;
}

.text-white {
  color: #fff;
}
</style>
