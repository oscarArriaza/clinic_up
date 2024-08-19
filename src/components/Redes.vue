<template>
    <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header bg-primary">
                <p class="h3 text-center text-light" id="modalTiendaLabel">
                    Mas Información
                </p>
            </div>
            <div class="modal-body bg-secondary" style="height: 353px; overflow-y: auto;">
                <div class="row">
                    <p class="h5 text-center col-sm-12">Redes</p>

                </div>
            </div>
            <div class="modal-footer bg-primary">
                <div class="row">
                    <button type="button" class="btn btn-danger" id="botonRegresarAlInventario" @click="cerrarRedes()">
                        Atras
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                POKEBALLMAX:15,
                POCIONESMAX:5,
                MINIMO:0,
                sumaBallsInventario:0,
                sumaPocionesInventario:0
            }
        },
        methods: {
            cerrarRedes()
            {
                this.$emit('cerrar-redes');
            }
        },
        props: {
            inventario: Object
        },
        created(){
        },
    }
</script>

<style>
    
</style>