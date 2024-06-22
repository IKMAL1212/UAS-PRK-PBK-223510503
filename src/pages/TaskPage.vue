<template>
  
  <div class="q-pa-md">
    <q-page>
      <h3>
      tugas 1 cara lihatnya di blok
      </h3>
      <q-list bordered padding>
        <a href="#" v-for="taskNumber in taskNumbers" :key="taskNumber" class="q-item" @click="goToTask(taskNumber)">
          {{ `Ini tugas  ${taskNumber}, Mau liat? silakan klik` }}

        </a>
      </q-list>
    </q-page>
  </div>
</template>

<script>
export default {
  data() {
    return {
      taskNumbers: [1, 2, 3, 4, 5, 6, 7]
    };
  },
  methods: {
    goToTask(taskNumber) {
      const taskLinks = {
        1: "https://tugas1-pbk-223510503-p3ml.vercel.app/",
        2: "https://tugas2pbk-223510503.vercel.app/",
        3: "https://223510503-ikmalardhiyaro-tugas3.vercel.app/",
        4: "https://tugas4-pbk-223510503-praktikum.vercel.app/",
        5: "https://tugas5-pbk-223510503.vercel.app/",
        6: "https://tugas6-pbk-223510503.vercel.app/",
        7: "https://tugas7-pbk-223510503.vercel.app/"
      };
      window.open(taskLinks[taskNumber], '_blank');
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Times+New+Roman&display=swap');

.q-pa-md {
  padding: 16px;
  background-image: url('../assets/Awan.png');
  background-size: cover;
  background-position: center;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  position: fixed;
  top: 50px;
  left: 0;
  right: 0;
  bottom: 0;
}

.q-list {
  max-width: 400px;
  margin: 0 auto;
  background: #f9fac6;
  border-radius: 10px;
  padding: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.q-item {
  display: block;
  padding: 12px 16px;
  border-radius: 5px;
  background-color: #ffffff;
  margin-bottom: 8px;
  cursor: pointer;
  transition: background-color 0.3s ease, box-shadow 0.3s ease;
  font-family: 'Times New Roman', Times, serif; 
  font-weight: 500;
  text-decoration: none;
  color: inherit;
}

.q-item:hover {
  background-color: #ea4e4e;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
}
</style>
