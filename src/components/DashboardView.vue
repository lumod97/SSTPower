<template>
  <b-row class="w-100">
    <b-col xs="2" sm="6" md="5" lg="5" xl="5">
      <human-body @parteChange="mostrar" @emitAccident="saveAccident" />
    </b-col>
    <b-col xs="10" sm="6" md="7" lg="7" xl="7">
      <accident-details :info-of="infoOf" :new-accident="newAccident" />
    </b-col>
  </b-row>
</template>

<script>
import AccidentDetails from "./AccidentDetails.vue";
import HumanBody from "./HumanBody.vue";

export default {
  data() {
    return {
      infoOf: "all",
      newAccident: [],
    };
  },
  components: {
    AccidentDetails,
    HumanBody,
  },
  methods: {
    mostrar(data) {
      this.infoOf = data;
    },
    saveAccident(newAccident) {
      this.newAccident = newAccident;
    },
  },
};
</script>