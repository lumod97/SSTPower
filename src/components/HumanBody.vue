<template>
  <div>
    <svg
      version="1.1"
      id="Capa_1"
      x="0px"
      y="0px"
      width="auto"
      height="auto"
      viewBox="0 0 168.066 168.066"
      style="enable-background: new 0 0 168.066 168.066"
      xmlns="http://www.w3.org/2000/svg"
    >
      <defs></defs>
      <!-- cabeza -->
      <path
        v-b-tooltip.hover.top="'Cabeza'"
        @mouseenter="mostrar('cabeza')"
        @dblclick="registerAccident('cabeza')"
        class="head"
        d="M 77.062 24.75 L 91.031 24.75 C 89.569 22.654 90.404 18.626 90.404 18.626 C 91.618 17.639 92.079 15.023 92.079 15.023 C 94.087 13.493 93.994 11.223 93.082 11.251 C 92.319 11.27 92.5 10.657 92.5 10.657 C 93.761 0.503 84.738 0 84.738 0 L 83.359 0 C 83.359 0 74.356 0.515 75.601 10.657 C 75.601 10.657 75.762 11.27 75.017 11.251 C 74.088 11.223 73.997 13.483 76.014 15.023 C 76.014 15.023 76.473 17.639 77.69 18.626 C 77.69 18.626 78.519 22.653 77.062 24.75 Z"
      ></path>
      <!-- pie derecho -->
      <path
        v-b-tooltip.hover.top="'Pie derecho'"
        @mouseenter="mostrar('pie derecho')"
        @dblclick="registerAccident('pie derecho')"
        title="pie"
        class="head"
        d="M 81.115 161.073 C 81.115 161.073 80.832 161.043 74.245 160.173 C 74.245 160.173 71.118 166.592 73.132 166.729 C 73.132 166.729 73.295 167.156 73.955 166.811 C 73.955 166.811 75.031 167.922 76.202 167.326 C 76.202 167.326 77.283 168.18 78.202 167.419 C 78.202 167.419 78.957 168.261 80.041 167.583 C 80.041 167.583 81.452 168.524 82.287 167.495 C 82.287 167.495 83.795 167.846 81.115 161.073 Z"
        style=""
      ></path>
      <!-- pie izquierdo -->
      <path
        v-b-tooltip.hover.top="'Pie izquierdo'"
        @mouseenter="mostrar('pie izquierdo')"
        @dblclick="registerAccident('pie izquierdo')"
        class="head"
        d="M 93.616 160.219 C 87.127 161.089 86.741 161.119 86.741 161.119 C 84.062 167.881 85.57 167.541 85.57 167.541 C 86.405 168.57 87.821 167.629 87.821 167.629 C 88.905 168.307 89.662 167.465 89.662 167.465 C 90.579 168.236 91.654 167.372 91.654 167.372 C 92.831 167.969 93.901 166.857 93.901 166.857 C 94.568 167.202 94.732 166.775 94.732 166.775 C 96.73 166.643 93.616 160.219 93.616 160.219 Z"
        style=""
      ></path>
      <!-- pierna derecha -->
      <path
        v-b-tooltip.hover.top="'Pierna derecha'"
        @mouseenter="mostrar('pierna derecha')"
        @dblclick="registerAccident('pierna derecha')"
        class="head"
        d="M 83.025 96.04 C 83.025 96.04 66.426 90.962 66.436 91.033 C 67.224 96.794 68.498 109.156 69.878 114.031 C 70.588 116.551 70.167 122.912 70.744 124.494 C 70.996 125.183 70.863 125.806 70.307 127.389 C 68.352 132.856 68.61 136.702 73.502 151.214 C 73.502 151.214 75.003 154.426 74.245 160.204 C 74.245 160.204 74.595 160.252 81.115 161.104 C 81.115 161.104 80.09 153.947 79.535 152.545 C 78.465 149.861 79.217 142.568 79.453 140.992 C 79.815 138.383 79.619 133.911 78.941 130.46 C 78.459 127.985 79.789 123.313 80.275 120.439 C 81.293 114.387 83.272 98.945 83.025 96.04 Z"
        style=""
      ></path>
      <!-- pierna izquierda -->
      <path
        v-b-tooltip.hover.top="'Pierna izquierda'"
        @mouseenter="mostrar('pierna izquierda')"
        @dblclick="registerAccident('pierna izquierda')"
        class="head"
        d="M 101.409 91.071 C 101.401 91.037 84.809 96.078 84.809 96.078 C 84.563 98.995 86.534 114.426 87.564 120.477 C 88.047 123.35 89.38 128.023 88.9 130.498 C 88.221 133.949 88.025 138.421 88.388 141.03 C 88.625 142.606 89.38 149.905 88.308 152.583 C 87.746 153.984 86.725 161.142 86.725 161.142 C 93.612 160.241 93.597 160.252 93.6 160.242 C 92.845 154.464 94.344 151.252 94.344 151.252 C 99.236 136.74 99.488 132.894 97.541 127.427 C 96.976 125.857 96.85 125.222 97.102 124.532 C 97.687 122.95 97.251 116.589 97.972 114.069 C 99.353 109.199 102.739 96.736 101.409 91.071 Z"
        style=""
      ></path>
      <!-- mano derecha -->
      <path
        v-b-tooltip.hover.top="'Mano derecha'"
        @mouseenter="mostrar('mano derecha')"
        @dblclick="registerAccident('mano derecha')"
        class="head"
        d="M 59.899 83.197 C 59.899 82.945 55.951 77.703 55.344 79.383 C 54.98 80.368 53.696 82.036 52.699 83.273 C 50.738 85.725 47.444 90.819 49.204 91.383 C 49.204 91.383 50.563 91.514 52.379 87.924 C 52.379 87.924 52.346 89.303 50.882 93.32 C 50.604 94.074 49.385 97.868 51.353 96.505 C 51.353 96.505 52.257 95.88 53.45 91.957 C 53.45 91.957 52.817 98.551 53.513 98.879 C 54.438 99.327 54.951 98.036 55.36 92.247 C 55.36 92.247 55.786 90.389 55.984 97.511 C 55.995 97.868 56.544 99.699 57.289 98.146 C 57.91 96.838 57.637 93.359 57.637 92.193 C 57.637 92.193 58.454 96.691 59.204 96.691 C 59.204 96.691 60.091 97.742 59.738 92.16 C 59.663 91.246 59.99 89.37 60.028 88.811 L 60.118 86.666 C 60.118 86.666 59.899 84.215 59.899 83.197 Z"
      ></path>
      <!-- mano izquierda -->
      <path
        v-b-tooltip.hover.top="'Mano izquierda'"
        @mouseenter="mostrar('mano izquierda')"
        @dblclick="registerAccident('mano izquierda')"
        class="head"
        d="M 115.389 83.272 C 114.39 82.036 113.115 80.355 112.746 79.382 C 112.139 77.702 108.15 82.955 108.15 83.197 C 108.15 84.219 107.929 86.666 107.929 86.666 L 108.019 88.811 C 108.061 89.37 108.369 91.246 108.313 92.16 C 107.959 97.73 108.845 96.691 108.845 96.691 C 109.598 96.691 110.413 92.193 110.413 92.193 C 110.413 93.353 110.129 96.833 110.76 98.146 C 111.521 99.69 112.054 97.869 112.067 97.511 C 112.263 90.389 112.689 92.247 112.689 92.247 C 113.095 98.026 113.609 99.327 114.529 98.879 C 115.229 98.54 114.594 91.957 114.594 91.957 C 115.788 95.858 116.695 96.505 116.695 96.505 C 118.66 97.868 117.442 94.064 117.166 93.32 C 115.7 89.302 115.667 87.924 115.667 87.924 C 117.474 91.525 118.843 91.383 118.843 91.383 C 120.647 90.818 117.331 85.725 115.389 83.272 Z"
      ></path>
      <!-- cuerpo -->
      <path
        v-b-tooltip.hover.top="'Cuerpo'"
        @mouseenter="mostrar('cuerpo')"
        @dblclick="registerAccident('cuerpo')"
        class="head"
        d="M 98.483 53.588 C 100.42 56.609 98.768 27.993 98.768 27.993 C 91.883 26.956 90.93 24.743 90.93 24.743 C 77.422 24.791 90.338 24.79 76.961 24.743 C 76.961 24.743 76.002 26.962 69.122 27.993 C 69.122 27.993 67.425 56.61 69.362 53.588 C 69.362 53.588 70.741 68.677 69.81 72.916 C 69.81 72.916 65.064 83.382 66.427 91.085 C 66.439 91.152 83.05 96.118 83.016 96.092 L 83.835 96.376 C 84.428 96.376 84.816 96.092 84.816 96.092 C 84.837 96.13 101.407 91.157 101.416 91.085 C 102.373 83.321 98.034 72.916 98.034 72.916 C 97.104 68.677 98.483 53.588 98.483 53.588 Z"
        style=""
      ></path>
      <!-- brazo derecho -->
      <path
        v-b-tooltip.hover.top="'Brazo derecho'"
        @mouseenter="mostrar('brazo derecho')"
        @dblclick="registerAccident('brazo derecho')"
        class="head"
        d="M 69.463 53.595 L 61.346 50.862 C 61.346 50.862 60.834 58.89 58.145 63.188 C 58.145 63.188 56.593 65.946 56.397 72.319 C 56.397 72.319 55.951 77.703 55.344 79.383 C 54.98 80.368 59.899 84.215 59.899 83.197 C 59.899 82.945 60.774 79.594 63.088 76.071 C 63.088 76.071 67.902 67.529 67.591 61.946 C 67.591 61.946 67.526 56.617 69.463 53.595 Z"
      ></path>
      <!-- brazo izquierdo -->
      <path
        v-b-tooltip.hover.top="'Brazo izquierdo'"
        @mouseenter="mostrar('brazo izquierdo')"
        @dblclick="registerAccident('brazo izquierdo')"
        class="head"
        d="M 108.165 83.106 C 108.165 84.128 113.13 80.264 112.761 79.291 C 112.154 77.611 111.705 72.227 111.705 72.227 C 111.518 65.854 109.959 63.096 109.959 63.096 C 107.269 58.787 106.766 50.77 106.766 50.77 L 98.599 53.504 C 100.536 56.525 100.47 61.855 100.47 61.855 C 100.153 67.433 104.968 75.98 104.968 75.98 C 107.288 79.515 108.165 82.864 108.165 83.106 Z"
      ></path>
      <!-- antebrazo derecho -->
      <path
        v-b-tooltip.hover.top="'Antebrazo derecho'"
        @mouseenter="mostrar('antebrazo derecho')"
        @dblclick="registerAccident('antebrazo derecho')"
        class="head"
        d="M 69.334 53.572 C 69.334 53.572 75.974 26.946 69.094 27.977 C 69.094 27.977 62.275 28.043 61.334 37.291 L 61.217 50.839 C 61.217 50.839 61.177 50.863 69.334 53.572 Z"
      ></path>
      <!-- antebrazo izquierdo -->
      <path
        v-b-tooltip.hover.top="'Antebrazo izquierdo'"
        @mouseenter="mostrar('antebrazo izquierdo')"
        @dblclick="registerAccident('antebrazo izquierdo')"
        class="head"
        d="M 98.61 53.479 C 106.81 50.739 106.777 50.745 106.777 50.745 L 106.655 37.197 C 105.726 27.95 98.895 27.884 98.895 27.884 C 92.01 26.847 98.61 53.479 98.61 53.479 Z"
      ></path>
    </svg>
    <!-- MODALS -->
    <modal-register-accident
      v-if="showRegisterModal"
      :parte-seleccionada="parteSeleccionada"
      @saveAccident="emitAccident"
      @hidden="showRegisterModal = false"
    />
  </div>
</template>

<style scoped>
.head:hover {
  fill: #ff0000a8;
  cursor: pointer;
}
</style>


<script>
import ModalRegisterAccident from "@/components/ModalRegisterAccident.vue";
export default {
  components: {
    ModalRegisterAccident,
  },
  data() {
    return {
      infoOf: "",
      showRegisterModal: false,
      parteSeleccionada: "",
    };
  },
  methods: {
    mostrar(parte) {
      this.$emit("parteChange", parte);
    },
    registerAccident(parte) {
      this.parteSeleccionada = parte;
      this.showRegisterModal = true;
    },
    emitAccident(newAccident){
      
      this.$emit('emitAccident',newAccident)
    }
  },
};
</script>