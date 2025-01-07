<template>
  <b-row class="w-100">
    <b-col xs="10" sm="6" md="7" lg="7" xl="7">
      <san-juan-map @parronSeleccionado="mostrarData"></san-juan-map>
    </b-col>
    <b-col xs="2" sm="6" md="5" lg="5" xl="5" v-if="plagas.length > 0" class="pt-5 ps-5">
      <h3> Plagas presentes en el parrón</h3>
      <div v-for="(item, index) in plagas" :key="index">
        <h5 class="mt-2">
          {{'🪲' + item}}
        </h5>
       </div>
    </b-col>
  </b-row>
</template>

<script>
// import AccidentDetails from "./AccidentDetails.vue";
// import HumanBody from "./HumanBody.vue";
import SanJuanMap from "./SanJuanMap.vue";

export default {
  data() {
    return {
      infoOf: "all",
      newAccident: [],
      plagas: []
    };
  },
  components: {
    // AccidentDetails,
    // HumanBody,
    SanJuanMap
  },
  methods: {
    mostrar(data) {
      this.infoOf = data;
    },
    saveAccident(newAccident) {
      this.newAccident = newAccident;
    },
    mostrarData(data){
      console.log(data)
      this.plagas = data.plagas
    }
  },
};
</script>