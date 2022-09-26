<script>

export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    somar() {
      this.contador++;
    },
    menos() {
      this.contador--;
    },
    zerar(){
      this.contador = 0
    },
  },
};



</script>


<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
    <small>
      <h1>Rise - Code Programin 2.0</h1>
    </small>
    <hr />

    <h2>Contador: {{ contador }}</h2>
    <button @click="somar()">+1</button>
    <button @click="menos()">-1</button>
    <button @click="zerar()">Zerar</button>
  </div>
</template>

<style scoped>
@import "./assets/base.css";

.container {
  text-align: center;
}

small {
  color: rgb(68, 66, 66);
}

h1 {
  font-weight: bolder;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
</style>