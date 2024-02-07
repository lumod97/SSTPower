<template>
  <b-card>
    <data-zona-afectada
      :data-accidentes="zonasAccidentes.filter((data) => data.zona == infoOf)"
    />
  </b-card>
</template>

<script>
import DataZonaAfectada from "./DataZonaAfectada.vue";
export default {
  components: {
    DataZonaAfectada,
  },
  data() {
    return {
      zonasAccidentes: [
        {
          zona: "cabeza",
          cantidad: 5,
          detalles: [
            {
              fecha: "2024-02-06",
              parte_afectada: "Ojo",
              gravedad: "Media",
            },
            {
              fecha: "2024-01-19",
              parte_afectada: "Cuello",
              gravedad: "Grave",
            },
            {
              fecha: "2024-01-02",
              parte_afectada: "Nariz",
              gravedad: "Grave",
            },
            {
              fecha: "2024-02-02",
              parte_afectada: "Oreja",
              gravedad: "Leve",
            },
            {
              fecha: "2024-01-20",
              parte_afectada: "Frente",
              gravedad: "Leve",
            },
          ],
        },
        {
          zona: "antebrazo izquierdo",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "antebrazo derecho",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "brazo izquierdo",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "brazo derecho",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "pierna izquierda",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "pierna derecha",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "pie izquierdo",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "pie derecho",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "mano izquierda",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "mano derecha",
          cantidad: 0,
          detalles: [
            
          ],
        },
        {
          zona: "cuerpo",
          cantidad: 0,
          detalles: [
            
          ],
        },
      ],
    };
  },
  props: {
    infoOf: {
      type: String,
      default: "all",
    },
    newAccident: {
        type: Object,
        require: false
    }
  },
  watch:{
    newAccident(newValue){
        console.log(newValue)
        if(newValue.lenght !== 0){
            this.zonasAccidentes.filter((zona)=>{
                if(zona.zona == newValue.zona){
                    zona.detalles.push(newValue)
                }
            }
            )
        }
    }
  }
};
</script>