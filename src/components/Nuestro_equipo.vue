<template>
    <Redes id="redes" hidden @cerrar-redes="cerrarRedes"></Redes>
    <div id="nuestroEquipo" class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header bg-primary">
                <img class="w-100" src="/public/media/imagenes/titulos/nuestro_equipo.png" alt="Nuestro Equipo" draggable="false">
            </div>
            <div class="modal-body bg-secondary" style="height: 353px; overflow-y: auto;">
                <div class="row">
                    <div class="col-sm-12 contenedorFlexible mb-3">
                        <div class="w-50 centrado">
                            <img class="w-100" src="/public/media/imagenes/fotos_de_perfil_empleados_de_clinicup/foto_de_perfil_doctora_jaisa_diaz.png" alt="Foto de perfil doctora Jaisa Diaz" draggable="false">
                        </div>
                        <div class="w-50 centrado">
                            <div class="ms-2">
                                <div class="text-center">
                                    <span class="text-light">
                                        <strong>
                                            Dra. Jaisa Díaz Bautista
                                        </strong>
                                    </span>
                                </div>
                                <div class="text-center">
                                    <span class="text-light">
                                        Cirujana Maxilofacial
                                    </span>
                                </div>
                                <div class="text-center">
                                    <button type="button" class="btn btn-warning btn-sm" @click="abrirMasInfo()">
                                        +Info
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 contenedorFlexible mb-3">
                        <div class="w-50 centrado">
                            <img class="w-100" src="/public/media/imagenes/fotos_de_perfil_empleados_de_clinicup/foto_de_perfil_doctora_jazmin_diaz_bautista.png" alt="Foto de perfil doctora Jazmin Diaz" draggable="false">
                        </div>
                        <div class="w-50 centrado">
                            <div class="ms-2">
                                <div class="text-center">
                                    <span class="text-light">
                                        <strong>
                                            Dra. Jazmín Díaz Bautista
                                        </strong>
                                    </span>
                                </div>
                                <div class="text-center">
                                    <span class="text-light">
                                        Especialistas en Tricologia y Microinjerto
                                    </span>
                                </div>
                                <div class="text-center">
                                    <button type="button" class="btn btn-warning btn-sm" @click="abrirMasInfo()">
                                        +Info
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 contenedorFlexible mb-3">
                        <div class="w-50 centrado">
                            <img class="w-100" src="/public/media/imagenes/fotos_de_perfil_empleados_de_clinicup/foto_de_perfil_doctora_rosa_bautista.png" alt="Foto de perfil doctora Rosa Bautista" draggable="false">
                        </div>
                        <div class="w-50 centrado">
                            <div class="ms-2">
                                <div class="text-center">
                                    <span class="text-light">
                                        <strong>
                                            Dra. Rosa Bautista
                                        </strong>
                                    </span>
                                </div>
                                <div class="text-center">
                                    <span class="text-light">
                                        Medicina de Familia
                                    </span>
                                </div>
                                <div class="text-center">
                                    <button type="button" class="btn btn-warning btn-sm" @click="abrirMasInfo()">
                                        +Info
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-12 contenedorFlexible mb-3">
                        <div class="w-50 centrado">
                            <img class="w-100" src="/public/media/imagenes/fotos_de_perfil_empleados_de_clinicup/foto_de_perfil_doctora_barbara_quevedo.png" alt="Foto de perfil doctora Barbara Quevedo" draggable="false">
                        </div>
                        <div class="w-50 centrado">
                            <div class="ms-2">
                                <div class="text-center">
                                    <span class="text-light">
                                        <strong>
                                            Dra. Barbara Quevedo
                                        </strong>
                                    </span>
                                </div>
                                <div class="text-center">
                                    <span class="text-light">
                                        Médico internista
                                    </span>
                                </div>
                                <div class="text-center">
                                    <button type="button" class="btn btn-warning btn-sm" @click="abrirMasInfo()">
                                        +Info
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="modal-footer bg-primary">
                <button type="button" class="btn btn-danger" id="botonCerrarModalNuestroEquipo" data-bs-dismiss="modal">
                    Atras
                </button>
            </div>
        </div>
    </div>
</template>

<script>
    import Redes from './Redes.vue'
    export default {
        data(){
            return {
            }
        },
        methods:{
            abrirMasInfo()
            {
                let nuestroEquipo = document.getElementById('nuestroEquipo');
                nuestroEquipo.setAttribute('hidden', "true");
                let redes = document.getElementById('redes');
                redes.removeAttribute('hidden');
            },
            cerrarRedes()
            {
                let nuestroEquipo = document.getElementById('nuestroEquipo');
                nuestroEquipo.removeAttribute('hidden');
                let redes = document.getElementById('redes');
                redes.setAttribute('hidden', "true");
            },
            actualizarInventario(inventarioActualizado)
            {
                this.inventarioDos.duskBall = inventarioActualizado.duskBall;
                this.inventarioDos.greatBall = inventarioActualizado.greatBall;
                this.inventarioDos.healBall = inventarioActualizado.healBall;
                this.inventarioDos.masterBall = inventarioActualizado.masterBall;
                this.inventarioDos.repeatBall = inventarioActualizado.repeatBall;
                this.inventarioDos.pocion = inventarioActualizado.pocion;
                this.inventarioDos.antidoto = inventarioActualizado.antidoto;

                let cantidadDuskBalls = document.getElementById('cantidadDuskBalls');
                cantidadDuskBalls.textContent="";
                cantidadDuskBalls.textContent=inventarioActualizado.duskBall;

                let cantidadGreatBalls = document.getElementById('cantidadGreatBalls');
                cantidadGreatBalls.textContent="";
                cantidadGreatBalls.textContent=inventarioActualizado.greatBall;

                let cantidadHealBalls = document.getElementById('cantidadHealBalls');
                cantidadHealBalls.textContent="";
                cantidadHealBalls.textContent=inventarioActualizado.healBall;

                let cantidadMasterBalls = document.getElementById('cantidadMasterBalls');
                cantidadMasterBalls.textContent="";
                cantidadMasterBalls.textContent=inventarioActualizado.masterBall;

                let cantidadRepeatBalls = document.getElementById('cantidadRepeatBalls');
                cantidadRepeatBalls.textContent="";
                cantidadRepeatBalls.textContent=inventarioActualizado.repeatBall;

                let cantidadPociones = document.getElementById('cantidadPociones');
                cantidadPociones.textContent="";
                cantidadPociones.textContent=inventarioActualizado.pocion;

                let cantidadAntidotos = document.getElementById('cantidadAntidotos');
                cantidadAntidotos.textContent="";
                cantidadAntidotos.textContent=inventarioActualizado.antidoto;
            }

        },
        components: {
            Redes
        },
        props: {
            inventario: Object
        },
        created(){
        },
    }
</script>

<style>
    .centrado
    {
        display:flex;
        align-items: center;
        justify-content: center;
    }
    .contenedorFlexible
    {
        display:flex;
    }
</style>