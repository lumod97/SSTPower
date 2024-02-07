<template>
  <div>
    <b-row class="w-100">
      <b-col cols="12" v-if="dataAccidentes.length == 0">
        Bienvenidos a SST Power App
      </b-col>
      <b-col cols="12" v-else>
        <div class="align-items-start w-100">
          <h3>
            {{ dataAccidentes[0].zona | capitalize }}
          </h3>
          <h5>
            {{
              "Existen " +
              dataAccidentes[0].cantidad +
              " accidentes reportados."
            }}
          </h5>
        </div>
        <!-- INFORMACION -->
        <b-card class="div-scroll">
          <template v-for="(detalle, index) in dataAccidentes[0].detalles">
            <b-alert
              :variant="getVariant(detalle.gravedad)"
              show
              :key="index"
              v-b-tooltip.hover.top="detalle.gravedad"
              class="cursor-pointer"
            >
              <span>{{ detalle.parte_afectada | capitalize }} </span>
              <span>{{ detalle.fecha }} </span>
            </b-alert>
          </template>
        </b-card>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  props: {
    dataAccidentes: {
      type: Array,
      require: false,
    },
  },
  methods: {
    getVariant(gravedad) {
      switch (gravedad) {
        case "Leve":
          return "primary";
        case "Media":
          return "warning";
        case "Grave":
          return "danger";
      }
    },
  },
};
</script>

<style>
.div-scroll {
  max-height: 70vh;
  overflow: auto;
}
</style>