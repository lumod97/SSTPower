<template>
    <b-modal ref="modal" @hidden="$emit('hidden')" hide-footer>
        <template #modal-header>
            {{ parteSeleccionada | capitalize }}
        </template>
        <div class="pl-3 pr-3">
            <b-row class="w-100">
                <b-col cols="12">
                    <b-form-group label=Trabajador>
                        <b-form-input v-model="newAccident.trabajador" disabled/>
                    </b-form-group>
                </b-col>
                <b-col cols="6">
                    <b-form-group label="DNI Trabajador">
                        <b-form-input v-model="newAccident.dni_trabajador"/>
                    </b-form-group>
                </b-col>
                <b-col cols="6">
                    <b-form-group label="Parte">
                        <b-form-input v-model="newAccident.parte_afectada"/>
                    </b-form-group>
                </b-col>
                <b-col cols="6">
                    <b-form-group label="Fecha">
                        <b-form-input type="date" v-model="newAccident.fecha"/>
                    </b-form-group>
                </b-col>
                <b-col cols="6">
                    <b-form-group label="Gravedad">
                        <b-form-select class="form-control" :options="['Leve','Media','Grave']" v-model="newAccident.gravedad"></b-form-select>
                    </b-form-group>
                </b-col>
            </b-row>
            <b-row class="w-100 mt-3 px-3">
                <b-button variant="secondary" @click="saveAccident()">
                    Guardar
                </b-button>
            </b-row>
        </div>
    </b-modal>
</template>

<script>
export default {
    data(){
        return{
            newAccident: {
                zona: this.parteSeleccionada,
                trabajador: '',
                dni_trabajador: '',
                parte_afectada: '',
                fecha: '',
                gravedad: '',
            }
        }
    },
    props:{
        parteSeleccionada:{
            type: String,
            require: true
        }
    },
    methods:{
        mostrarModal(){
            this.$refs.modal.show()
        },
        ocultarModal(){
            this.$refs.modal.hide()
        },
        saveAccident(){
            this.$emit('saveAccident', this.newAccident)
            this.ocultarModal()
        }
    },
    mounted(){
        this.mostrarModal()
    }
}
</script>