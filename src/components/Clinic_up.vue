<template>
    <header style="height: 118px;">
        <nav class="navbar navbar-expand-lg bg-primary fixed-top" data-bs-theme="dark">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">
                    <img src="/media/imagenes/logos/logo_0.png" id="logo" alt="Logo de Clinic Up" width="130vw" height="60vh" class="d-inline-block align-top" draggable="false">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarColor01">
                    <ul class="navbar-nav me-auto">
                        <li class="nav-item">
                            <a class="nav-link" href="#inicio">
                                Inicio
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#objetivo">
                                Nuestro objetivo
                            </a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="tratamientos" role="button" aria-haspopup="true" aria-expanded="false">
                                Tratamientos
                            </a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#minoxidil" @click="abrirTratamiento($event.target.textContent)">Minoxidil</a>
                                <a class="dropdown-item" href="#plasmaRicoEnPlaquetas" @click="abrirTratamiento('PlasmaRicoEnPlaquetas')">
                                    Plasma rico en plaquetas
                                </a>
                                <a class="dropdown-item" href="#mesoterapiaDeCorticoides" @click="abrirTratamiento('MesoterapiaDeCorticoides')">
                                    Mesoterapia de corticoides
                                </a>
                                <a class="dropdown-item" href="#mesoterapiaAntiandrogenica" @click="abrirTratamiento('MesoterapiaAntiandrogenica')">
                                    Mesoterapia antiandrogénica
                                </a>
                                <a class="dropdown-item" href="#microneedling" @click="abrirTratamiento($event.target.textContent)">Microneedling</a>
                                <a class="dropdown-item" href="#">
                                    Oxigeno terapia
                                </a>
                                <a class="dropdown-item" href="#">
                                    Luz
                                </a>
                            </div>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
                                Armonización facial
                            </a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#">
                                    Bótox facial
                                </a>
                                <a class="dropdown-item" href="#">
                                    Blefaroplastia
                                </a>
                                <a class="dropdown-item" href="#">
                                    Rinomodelación
                                </a>
                                <a class="dropdown-item" href="#">
                                    Bichectomía
                                </a>
                            </div>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#galeria">
                                Galería
                            </a>
                        </li>
                        <!--<li class="nav-item">
                            <a class="nav-link" href="#">
                                Nuestro equipo
                            </a>
                        </li>-->
                        <li class="nav-item">
                            <a class="nav-link" href="#">
                                Contacto
                            </a>
                        </li>
                        <!--<li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">Dropdown</a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#">Action</a>
                                <a class="dropdown-item" href="#">Another action</a>
                                <a class="dropdown-item" href="#">Something else here</a>
                                <div class="dropdown-divider"></div>
                                <a class="dropdown-item" href="#">Separated link</a>
                            </div>
                        </li>-->
                    </ul>
                </div>
            </div>
        </nav>
        <div id="inicio"></div>
    </header>
    <section style="height: auto;">


        
        <div id="quienesSomos">
            <div class="w-75 h-75 row" id="titulo">
                <p class="text-light h1 text-center col-sm-12">
                    <strong>Centro Especializado</strong>
                </p>
                <p class="text-light h1 text-start col-sm-12" title="Cirugia Maxilofacial">
                    -Cirugía Maxilofacial
                </p>
                <p class="text-light h1 text-start col-sm-12">
                    -Armonización orofacial
                </p>
                <p class="text-light h1 text-start col-sm-12">
                    -Tricología
                </p>
                <p class="text-light h1 text-start col-sm-12">
                    -Cirugía Capilar
                </p>
                <p class="text-light h1 text-start col-sm-12">
                    -Telemedicina
                </p>
            </div>
        </div>


        <div id="objetivo">
            <div class="w-75 h-75 row" id="parrafoObjetivo">
                <p class="text-light h1 text-center">
                    Nuestro objetivo es acompañarte para que te sientas mejor. Queremos estar a tu lado en este proceso, con un abordaje sumamente especializado, de la mano de la última evidencia científica y la mejor tecnología disponible.
                </p>
            </div>
            <div id="minoxidil"></div>
            <div id="plasmaRicoEnPlaquetas"></div>
        </div>
        <div id="mesoterapiaDeCorticoides"></div>
        <div id="mesoterapiaAntiandrogenica"></div>
        
        <div id="tratamientos" class="pt-1">
            <p class="h1 text-center text-primary">
                Tratamientos
            </p>
            <div class="accordion accordion-flush" id="accordionFlushExample">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMinoxidil" class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoUno" aria-expanded="false" aria-controls="colapsarFlujoUno">
                            Minoxidil
                        </button>
                    </h2>
                    <div id="colapsarFlujoUno" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            El
                            <code>
                                minoxidil
                            </code>
                            es un medicamento que se utiliza principalmente para el tratamiento de la caída del cabello y la promoción del crecimiento capilar. Fue originalmente desarrollado como un medicamento oral para tratar la hipertensión (presión arterial alta), pero se descubrió que uno de sus efectos secundarios era el crecimiento del cabello. Esto llevó al desarrollo de su forma tópica para tratar problemas de pérdida de cabello.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonPlasmaRicoEnPlaquetas" class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDos" aria-expanded="false" aria-controls="colapsarFlujoDos">
                            Plasma rico en plaquetas
                        </button>
                    </h2>
                    <div id="colapsarFlujoDos" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            El
                            <code>
                                tratamiento de Plasma Rico en Plaquetas (PRP)
                            </code>
                            es una terapia médica que utiliza las propias plaquetas del paciente para promover la curación y la regeneración de tejidos. Este tratamiento se ha utilizado en una variedad de campos médicos, incluidos la ortopedia, la medicina estética, la dermatología y la medicina deportiva.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMesoterapiaDeCorticoides" class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTres" aria-expanded="false" aria-controls="colapsarFlujoTres">
                            Mesoterapia de corticoides
                        </button>
                    </h2>
                    <div id="colapsarFlujoTres" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            La
                            <code>
                                mesoterapia de corticoides
                            </code>
                            es un tratamiento médico que implica la inyección de medicamentos corticosteroides en las capas superficiales de la piel o en el tejido subcutáneo. Los corticosteroides son fármacos antiinflamatorios potentes que se utilizan para tratar una variedad de condiciones médicas, particularmente aquellas que involucran inflamación.
                        </div>
                    </div>
                    <div id="microneedling"></div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMesoterapiaAntiandrogenica" class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCuatro" aria-expanded="false" aria-controls="colapsarFlujoCuatro">
                            Mesoterapia antiandrogénica
                        </button>
                    </h2>
                    <div id="colapsarFlujoCuatro" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            La
                            <code>
                                mesoterapia antiandrogénica
                            </code>
                            es un tratamiento que utiliza la técnica de mesoterapia para administrar medicamentos antiandrogénicos directamente en el cuero cabelludo o la piel. Este tratamiento se utiliza principalmente para abordar problemas relacionados con la pérdida de cabello, como la alopecia androgenética (calvicie de patrón masculino o femenino), y otras condiciones influenciadas por los andrógenos (hormonas sexuales masculinas).
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMicroneedling" class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCinco" aria-expanded="false" aria-controls="colapsarFlujoCinco">
                            Microneedling
                        </button>
                    </h2>
                    <div id="colapsarFlujoCinco" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            El <code>microneedling</code>, también conocido como terapia de inducción de colágeno, es un tratamiento estético que utiliza agujas diminutas para crear microperforaciones en la piel. Estas pequeñas heridas desencadenan la respuesta natural de curación del cuerpo, lo que resulta en la producción de nuevo colágeno y elastina, dos componentes cruciales para una piel saludable y de apariencia joven.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                    <button class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSeis" aria-expanded="false" aria-controls="colapsarFlujoSeis">
                        Oxigeno terapia
                    </button>
                    </h2>
                    <div id="colapsarFlujoSeis" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            Placeholder content for this accordion, which is intended to demonstrate the
                            <code>.accordion-flush</code>
                            class. This is the third item's accordion body. Nothing more exciting happening here in terms of content, but just filling up the space to make it look, at least at first glance, a bit more representative of how this would look in a real-world application.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                    <button class="accordion-button collapsed text-primary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSiete" aria-expanded="false" aria-controls="colapsarFlujoSiete">
                        Luz
                    </button>
                    </h2>
                    <div id="colapsarFlujoSiete" class="accordion-collapse collapse text-primary" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            Placeholder content for this accordion, which is intended to demonstrate the
                            <code>.accordion-flush</code>
                            class. This is the third item's accordion body. Nothing more exciting happening here in terms of content, but just filling up the space to make it look, at least at first glance, a bit more representative of how this would look in a real-world application.
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div id="galeria" class="carousel slide">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#galeria" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#galeria" data-bs-slide-to="1" aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#galeria" data-bs-slide-to="2" aria-label="Slide 3"></button>
                <button type="button" data-bs-target="#galeria" data-bs-slide-to="3" aria-label="Slide 4"></button>
                <button type="button" data-bs-target="#galeria" data-bs-slide-to="4" aria-label="Slide 5"></button>
            </div>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="/media/imagenes/imagenes_negocio/9.png" class="d-block w-100" alt="..." dragable="false">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>First slide label</h5>
                        <p>Some representative placeholder content for the first slide.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="/media/imagenes/imagenes_negocio/7.png" class="d-block w-100" alt="..." draggable="false">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Second slide label</h5>
                        <p>Some representative placeholder content for the second slide.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="/media/imagenes/imagenes_negocio/8.png" class="d-block w-100" alt="..." draggable="false">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Third slide label</h5>
                        <p>Some representative placeholder content for the third slide.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="/media/imagenes/imagenes_negocio/1.png" class="d-block w-100" alt="..." draggable="false">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Third slide label</h5>
                        <p>Some representative placeholder content for the third slide.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="/media/imagenes/imagenes_negocio/3.png" class="d-block w-100" alt="..." draggable="false">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Third slide label</h5>
                        <p>Some representative placeholder content for the third slide.</p>
                    </div>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#galeria" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#galeria" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>

        
    </section>
    <footer class="bg-primary text-end">
        <a href="https://www.instagram.com/clinic.up.bydb/" target="_blank">
            <img src="/media/imagenes/logos_empresas_de_terceros/instagram.png" alt="Logo de Instagram" width="50vw" height="50vh" draggable="false">
        </a>
    </footer>
</template>

<script>
    export default {
        data(){
            return {

            }
        },
        methods: {
            abrirTratamiento(tratamiento){
                let boton="boton"+tratamiento;
                let botonTratamiento=document.getElementById(boton);
                botonTratamiento.click();
            }
        },
        created(){

        },
    }
</script>

<style>
    #quienesSomos
    {
        background-image: url('/media/imagenes/imagenes_negocio/1.png');
        background-size: cover;
        background-position: center;
        height: 100vh;
    
        display:flex;
        align-items: center;
        justify-content: center;
    }
    #titulo
    {
        /*height: 500px;*/
        background-color: rgba(193, 166, 137, 0.697);
    }
    #objetivo
    {
        background-image: url('/media/imagenes/imagenes_negocio/3.png');
        background-size: cover;
        background-position: center;
        height: 100vh;
    
        display:flex;
        align-items: center;
        justify-content: center;
    }
    #parrafoObjetivo
    {
        display:flex;
        align-items: center;
        justify-content: center;
        /*height: 500px;*/
        /*background-color: rgba(255, 250, 243, 0.755);*/
        background-color: rgba(72, 133, 137, 0.682);
    }
    #tratamientos
    {
        background-color:rgb(255, 250, 243);
        /*background-color: rgba(193, 166, 137, 0.697);*/
    }
</style>