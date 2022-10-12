<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125" />
    <small>
      <h1>Hola desde VUE.js 3</h1>
    </small>
    <hr />

    <h2>Contador {{ contador }}</h2>
    <button @click="incrementar()" type="button" class="btn btn-success ">+1</button>
    <button @click="disminuir()"   type="button" class="btn btn-success ">-1</button>
    <button @click="resetear()"       type="button" class="btn btn-success ">Reset</button>

    <button type="button" class="btn btn-success" data-bs-toggle="modal" data-bs-target="#exampleModal">Moises Yosua Antonio Flores</button>
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLabel">Hola</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body"> DSM 4°B</div>
          <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data: () => ({
      contador: 500,
    }),
    methods: {
      saludar() {
        console.log("Hola !");
      },
      incrementar() {
        this.contador++;
      },
      disminuir() {
        this.contador--;
      },
      resetear() {
        this.contador = 500;
      },
    },
  };
</script>
  
<style scoped>
.container {
  text-align: center;
}
small {
  color: #666;
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
  margin: 0px 8px;
}
</style>
  
