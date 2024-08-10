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
                                Tratamientos capilares
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
                                <a class="dropdown-item" href="#oxigenoTerapia" @click="abrirTratamiento($event.target.textContent)">Oxigenoterapia</a>
                                <a class="dropdown-item" href="#luz" @click="abrirTratamiento($event.target.textContent)">Luz</a>
                            </div>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="armonizacionFacial" role="button" aria-haspopup="true" aria-expanded="false">
                                Armonización facial
                            </a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#botoxFacial" @click="abrirTratamiento('BotoxFacial')">
                                    Bótox facial
                                </a>
                                <a class="dropdown-item" href="#blefaroplastia" @click="abrirTratamiento($event.target.textContent)">Blefaroplastia</a>
                                <a class="dropdown-item" href="#rinomodelacion" @click="abrirTratamiento('Rinomodelacion')">
                                    Rinomodelación
                                </a>
                                <a class="dropdown-item" href="#bichectomia" @click="abrirTratamiento('Bichectomia')">
                                    Bichectomía
                                </a>
                            </div>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="telemedicina" role="button" aria-haspopup="true" aria-expanded="false">
                                Telemedicina
                            </a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#" @click="abrirTratamiento('ConsultasMaxilofaciales')">
                                    Consultas Maxilofaciales
                                </a>
                                <a class="dropdown-item" href="#" @click="abrirTratamiento('ConsultasCapilares')">
                                    Consultas Capilares
                                </a>
                                <a class="dropdown-item" href="#" @click="abrirTratamiento('ConsultasDeMedicinaInterna')">
                                    Consultas de Medicina Interna
                                </a>
                                <a class="dropdown-item" href="#" @click="abrirTratamiento('ConsultasDeMedicinaDeFamilia')">
                                    Consultas de Medicina de Familia
                                </a>
                                <a class="dropdown-item" href="#" @click="abrirTratamiento('ConsultasDeMedicinaGeneral')">
                                    Consultas de Medicina General
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
                            <a class="nav-link" href="#contacto">
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
            <div class="w-75 h-75 row" id="titulo" title="Centro especializado">
                <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/centro_especializado.png" alt="titulo de la seccion inicio" draggable="false">
                <img class="w-100 d-none d-lg-block" src="/public/media/imagenes/titulos/centro_especializado.png" alt="titulo de la seccion inicio" draggable="false">
                <p class="text-light h2 text-start col-sm-12">
                    -Cirugía Maxilofacial
                </p>
                <p class="text-light h2 text-start col-sm-12">
                    -Armonización orofacial
                </p>
                <p class="text-light h2 text-start col-sm-12">
                    -Tricología
                </p>
                <p class="text-light h2 text-start col-sm-12">
                    -Cirugía Capilar
                </p>
                <p class="text-light h2 text-start col-sm-12">
                    -Telemedicina
                </p>
            </div>
        </div>


        <div id="objetivo">
            <div class="w-75 h-75 row" id="parrafoObjetivo" title="Nuestro objetivo">
                <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/nuestro_objetivo.png" alt="titulo de la seccion nuestro objetivo" draggable="false">
                <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/titulos/nuestro_objetivo.png" alt="titulo de la seccion nuestro objetivo" draggable="false">
                <p class="text-light h2 text-center">
                    Es acompañarte para que te sientas mejor. Queremos estar a tu lado en este proceso, con un abordaje sumamente especializado, de la mano de la última evidencia científica y la mejor tecnología disponible.
                </p>
            </div>
            <div id="minoxidil"></div>
            <div id="plasmaRicoEnPlaquetas"></div>
        </div>
        <div id="mesoterapiaDeCorticoides"></div>
        <div id="mesoterapiaAntiandrogenica"></div>
        
        <div id="tratamientos" class="pt-1 bg-light" title="Tratamientos">
            <div class="tituloSeccion">
                <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/titulos/tratamientos.png" alt="titulo de la seccion tratamientos capilares palabra tratamientos" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/tratamientos.png" alt="titulo de la seccion tratamientos capilares palabra tratamientos" draggable="false">
            </div>
            <div class="tituloSeccion">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/capilares.png" alt="titulo de la seccion tratamientos capilares palabra capilares" draggable="false">
                <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/titulos/capilares.png" alt="titulo de la seccion tratamientos capilares palabra capilares" draggable="false">
            </div>
            <div class="accordion accordion-flush" id="accordionFlushUno">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMinoxidil" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoUno" aria-expanded="false" aria-controls="colapsarFlujoUno">
                            Minoxidil
                        </button>
                    </h2>
                    <div id="colapsarFlujoUno" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
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
                    <div id="microneedling"></div>
                    <div id="oxigenoTerapia"></div>
                    <div id="luz"></div>
                    <h2 class="accordion-header">
                        <button id="botonPlasmaRicoEnPlaquetas" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDos" aria-expanded="false" aria-controls="colapsarFlujoDos">
                            Plasma rico en plaquetas
                        </button>
                    </h2>
                    <div id="colapsarFlujoDos" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
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
                        <button id="botonMesoterapiaDeCorticoides" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTres" aria-expanded="false" aria-controls="colapsarFlujoTres">
                            Mesoterapia de corticoides
                        </button>
                    </h2>
                    <div id="colapsarFlujoTres" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            La
                            <code>
                                mesoterapia de corticoides
                            </code>
                            es un tratamiento médico que implica la inyección de medicamentos corticosteroides en las capas superficiales de la piel o en el tejido subcutáneo. Los corticosteroides son fármacos antiinflamatorios potentes que se utilizan para tratar una variedad de condiciones médicas, particularmente aquellas que involucran inflamación.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonMesoterapiaAntiandrogenica" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCuatro" aria-expanded="false" aria-controls="colapsarFlujoCuatro">
                            Mesoterapia antiandrogénica
                        </button>
                    </h2>
                    <div id="colapsarFlujoCuatro" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
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
                    <div id="botoxFacial"></div>
                    <div id="blefaroplastia"></div>
                    <h2 class="accordion-header">
                        <button id="botonMicroneedling" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCinco" aria-expanded="false" aria-controls="colapsarFlujoCinco">
                            Microneedling
                        </button>
                    </h2>
                    <div id="colapsarFlujoCinco" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            El <code>microneedling</code>, también conocido como terapia de inducción de colágeno, es un tratamiento estético que utiliza agujas diminutas para crear microperforaciones en la piel. Estas pequeñas heridas desencadenan la respuesta natural de curación del cuerpo, lo que resulta en la producción de nuevo colágeno y elastina, dos componentes cruciales para una piel saludable y de apariencia joven.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonOxigenoterapia" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSeis" aria-expanded="false" aria-controls="colapsarFlujoSeis">
                            Oxigenoterapia
                        </button>
                    </h2>
                    <div id="colapsarFlujoSeis" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            La
                            <code>
                                oxigenoterapia
                            </code>
                            es un tratamiento médico que consiste en suministrar oxígeno adicional a una persona para aumentar los niveles de oxígeno en la sangre. Se utiliza en una variedad de condiciones médicas donde los niveles de oxígeno en el cuerpo son insuficientes.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonLuz" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSiete" aria-expanded="false" aria-controls="colapsarFlujoSiete">
                            Luz
                        </button>
                    </h2>
                    <div id="colapsarFlujoSiete" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            El <code>tratamiento con luz</code>, también conocido como fototerapia o terapia de luz, es un procedimiento médico que utiliza luz para tratar diversas condiciones de salud, tanto físicas como psicológicas. Existen diferentes tipos de tratamientos con luz, que varían según el espectro de luz utilizado (ultravioleta, visible, infrarrojo) y la condición a tratar.
                        </div>
                    </div>
                </div>
                <div id="rinomodelacion"></div>
                <div id="bichectomia"></div>
                <!--<div id="oxigenoTerapia"></div>-->
            </div>
        </div>

        <div id="armonizacionFacial" class="pt-1 bg-secondary" title="Armonización Facial">
            <div class="tituloSeccion mb-1">
                <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/titulos/armonizacion.png" alt="titulo de la seccion armonizacion facial palabra armonizacion" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/armonizacion.png" alt="titulo de la seccion armonizacion facial palabra armonizacion" draggable="false">
            </div>
            <div class="tituloSeccion">
                <img class="w-25 d-block d-lg-none" src="/public/media/imagenes/titulos/facial.png" alt="titulo de la seccion armonizacion facial palabra facial" draggable="false">
                <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/titulos/facial.png" alt="titulo de la seccion armonizacion facial palabra facial" draggable="false">
            </div>
            <div class="accordion accordion-flush" id="accordionFlushDos">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonBotoxFacial" class="accordion-button collapsed text-light bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOcho" aria-expanded="false" aria-controls="colapsarFlujoOcho">
                            Bótox facial
                        </button>
                    </h2>
                    <div id="colapsarFlujoOcho" class="accordion-collapse collapse text-light bg-secondary" data-bs-parent="#accordionFlushDos">
                        <div class="accordion-body">
                            El tratamiento de
                            <code>
                                Bótox facial
                            </code>
                            es un procedimiento estético no quirúrgico que implica la inyección de toxina botulínica tipo A en los músculos faciales. Este tratamiento es ampliamente utilizado para reducir la apariencia de arrugas y líneas de expresión en la cara, proporcionando un aspecto más suave y rejuvenecido.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonBlefaroplastia" class="accordion-button collapsed text-light bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoNueve" aria-expanded="false" aria-controls="colapsarFlujoNueve">
                            Blefaroplastia
                        </button>
                    </h2>
                    <div id="colapsarFlujoNueve" class="accordion-collapse collapse text-light bg-secondary" data-bs-parent="#accordionFlushDos">
                        <div class="accordion-body">
                            La
                            <code>
                                blefaroplastia
                            </code>
                            es un procedimiento quirúrgico estético o reconstructivo que se realiza en los párpados para corregir problemas como el exceso de piel, bolsas de grasa, y otros signos de envejecimiento en la zona de los ojos. El objetivo principal de la blefaroplastia es mejorar la apariencia de los párpados y, en algunos casos, mejorar la visión obstruida por el exceso de piel.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonRinomodelacion" class="accordion-button collapsed text-light bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDiez" aria-expanded="false" aria-controls="colapsarFlujoDiez">
                            Rinomodelación
                        </button>
                    </h2>
                    <div id="colapsarFlujoDiez" class="accordion-collapse collapse text-light bg-secondary" data-bs-parent="#accordionFlushDos">
                        <div class="accordion-body">
                            La 
                            <code>
                                rinomodelación
                            </code>
                            es un procedimiento estético no quirúrgico diseñado para modificar la forma de la nariz mediante la inyección de materiales de relleno dérmico, como ácido hialurónico o hidroxiapatita de calcio. A diferencia de la rinoplastia, que es una cirugía para cambiar la estructura de la nariz, la rinomodelación permite realizar ajustes en la forma de la nariz sin necesidad de una operación quirúrgica.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonBichectomia" class="accordion-button collapsed text-light bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOnce" aria-expanded="false" aria-controls="colapsarFlujoOnce">
                            Bichectomía
                        </button>
                    </h2>
                    <div id="colapsarFlujoOnce" class="accordion-collapse collapse text-light bg-secondary" data-bs-parent="#accordionFlushDos">
                        <div class="accordion-body">
                            La
                            <code> 
                                bichectomía
                            </code>
                            es un procedimiento estético quirúrgico que consiste en la extracción de las bolsas de Bichat, que son acumulaciones de grasa situadas en las mejillas, entre los músculos de la cara. Estas bolsas no tienen una función específica y su tamaño puede variar de una persona a otra. La cirugía se realiza para afinar el rostro y dar una apariencia más estilizada o esculpida.
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div id="telemedicina" class="pt-1 bg-light" title="Telemedicina">
            <div class="tituloSeccion">
                <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/titulos/telemedicina.png" alt="titulo de la seccion armonizacion facial palabra armonizacion" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/telemedicina.png" alt="titulo de la seccion armonizacion facial palabra armonizacion" draggable="false">
            </div>
            <div class="accordion accordion-flush" id="accordionFlushTres">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonConsultasMaxilofaciales" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDoce" aria-expanded="false" aria-controls="colapsarFlujoDoce">
                            Consultas Maxilofaciales
                        </button>
                    </h2>
                    <div id="colapsarFlujoDoce" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushTres">
                        <div class="accordion-body">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ullamcorper ac metus at mollis. Phasellus imperdiet, ex tempus laoreet dignissim, justo est porttitor mi, id mollis nibh ex at nibh. Duis sed ipsum dictum, varius arcu at, facilisis velit. Vivamus nec tortor pretium, ornare nunc et, auctor felis. Aliquam elementum molestie imperdiet. Etiam ac fringilla orci. Vestibulum posuere id risus nec maximus. Morbi lobortis consectetur posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Donec non leo mauris. Ut viverra consectetur augue, quis porttitor metus facilisis in. Duis bibendum lectus id eleifend mattis. Morbi dapibus hendrerit pharetra. Ut semper interdum dolor, sit amet dignissim nunc aliquam eu.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonConsultasCapilares" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTrece" aria-expanded="false" aria-controls="colapsarFlujoTrece">
                            Consultas Capilares
                        </button>
                    </h2>
                    <div id="colapsarFlujoTrece" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushTres">
                        <div class="accordion-body">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ullamcorper ac metus at mollis. Phasellus imperdiet, ex tempus laoreet dignissim, justo est porttitor mi, id mollis nibh ex at nibh. Duis sed ipsum dictum, varius arcu at, facilisis velit. Vivamus nec tortor pretium, ornare nunc et, auctor felis. Aliquam elementum molestie imperdiet. Etiam ac fringilla orci. Vestibulum posuere id risus nec maximus. Morbi lobortis consectetur posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Donec non leo mauris. Ut viverra consectetur augue, quis porttitor metus facilisis in. Duis bibendum lectus id eleifend mattis. Morbi dapibus hendrerit pharetra. Ut semper interdum dolor, sit amet dignissim nunc aliquam eu.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonConsultasDeMedicinaInterna" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCatorce" aria-expanded="false" aria-controls="colapsarFlujoCatorce">
                            Consultas de Medicina Interna
                        </button>
                    </h2>
                    <div id="colapsarFlujoCatorce" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushTres">
                        <div class="accordion-body">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ullamcorper ac metus at mollis. Phasellus imperdiet, ex tempus laoreet dignissim, justo est porttitor mi, id mollis nibh ex at nibh. Duis sed ipsum dictum, varius arcu at, facilisis velit. Vivamus nec tortor pretium, ornare nunc et, auctor felis. Aliquam elementum molestie imperdiet. Etiam ac fringilla orci. Vestibulum posuere id risus nec maximus. Morbi lobortis consectetur posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Donec non leo mauris. Ut viverra consectetur augue, quis porttitor metus facilisis in. Duis bibendum lectus id eleifend mattis. Morbi dapibus hendrerit pharetra. Ut semper interdum dolor, sit amet dignissim nunc aliquam eu.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonConsultasDeMedicinaDeFamilia" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoQuince" aria-expanded="false" aria-controls="colapsarFlujoQuince">
                            Consultas de Medicina de Familia
                        </button>
                    </h2>
                    <div id="colapsarFlujoQuince" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushTres">
                        <div class="accordion-body">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ullamcorper ac metus at mollis. Phasellus imperdiet, ex tempus laoreet dignissim, justo est porttitor mi, id mollis nibh ex at nibh. Duis sed ipsum dictum, varius arcu at, facilisis velit. Vivamus nec tortor pretium, ornare nunc et, auctor felis. Aliquam elementum molestie imperdiet. Etiam ac fringilla orci. Vestibulum posuere id risus nec maximus. Morbi lobortis consectetur posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Donec non leo mauris. Ut viverra consectetur augue, quis porttitor metus facilisis in. Duis bibendum lectus id eleifend mattis. Morbi dapibus hendrerit pharetra. Ut semper interdum dolor, sit amet dignissim nunc aliquam eu.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonConsultasDeMedicinaGeneral" class="accordion-button collapsed text-primary bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDieciseis" aria-expanded="false" aria-controls="colapsarFlujoDieciseis">
                            Consultas de Medicina General
                        </button>
                    </h2>
                    <div id="colapsarFlujoDieciseis" class="accordion-collapse collapse text-primary bg-light" data-bs-parent="#accordionFlushTres">
                        <div class="accordion-body">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ullamcorper ac metus at mollis. Phasellus imperdiet, ex tempus laoreet dignissim, justo est porttitor mi, id mollis nibh ex at nibh. Duis sed ipsum dictum, varius arcu at, facilisis velit. Vivamus nec tortor pretium, ornare nunc et, auctor felis. Aliquam elementum molestie imperdiet. Etiam ac fringilla orci. Vestibulum posuere id risus nec maximus. Morbi lobortis consectetur posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Donec non leo mauris. Ut viverra consectetur augue, quis porttitor metus facilisis in. Duis bibendum lectus id eleifend mattis. Morbi dapibus hendrerit pharetra. Ut semper interdum dolor, sit amet dignissim nunc aliquam eu.
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="bg-secondary" title="Galería">
            <div class="tituloSeccion">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/galeria.png" alt="titulo de la seccion galería" draggable="false">
                <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/titulos/galeria.png" alt="titulo de la seccion galería" draggable="false">
            </div>
            <div id="carrusel" class="carousel slide">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="1" aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="2" aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="3" aria-label="Slide 4"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="4" aria-label="Slide 5"></button>
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
                <button class="carousel-control-prev" type="button" data-bs-target="#carrusel" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carrusel" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>

        <div id="contacto" class="bg-light container pt-1" title="contacto">
            <div class="tituloSeccion bg-light">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/contacto.png" alt="titulo de la seccion contacto" draggable="false">
                <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/titulos/contacto.png" alt="titulo de la seccion contacto" draggable="false">
            </div>
            <div class="row bg-light">
                <div class="col-sm-12 col-md-6 contenedorFlexible mt-3">
                    <div class="w-25 centrado">
                        <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/telefono.png" alt="Icono teléfono" draggable="false">
                        <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/telefono.png" alt="Icono teléfono" draggable="false">
                    </div>
                    <p class="h2 text-primary w-75">
                        809-638-7607
                    </p>
                    <!--<img class="w-25 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/telefono.png" alt="Icono teléfono" draggable="false">
                    <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/telefono.png" alt="Icono teléfono" draggable="false">-->
                </div>
                <a href="https://api.whatsapp.com/message/VPCDBHGXRHNME1?autoload=1&app_absent=0" target="_blank" class="col-sm-12 col-md-6 contenedorFlexible mt-3">
                    <div class="w-25 centrado">
                        <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/whatsapp.png" alt="Icono whatsapp" draggable="false">
                        <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/whatsapp.png" alt="Icono whatsapp" draggable="false">
                    </div>
                    <p class="h2 text-primary w-75">
                        829-705-7607
                    </p>
                </a>
                <a href="https://www.instagram.com/clinic.up.bydb/" target="_blank" class="col-sm-12 col-md-6 contenedorFlexible mt-3">
                    <div class="w-25 centrado">
                        <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/instagram_1.png" alt="Icono instagram" draggable="false">
                        <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/instagram_1.png" alt="Icono instagram" draggable="false">
                    </div>
                    <p class="h2 text-primary w-75">
                        @clinic.up.byDB
                    </p>
                </a>
                <div class="col-sm-12 col-md-6 contenedorFlexible mt-3">
                    <div class="w-25 centrado">
                        <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/correo.png" alt="Icono correo" draggable="false">
                        <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/correo.png" alt="Icono correo" draggable="false">
                    </div>
                    <p class="h2 text-primary w-75 enUnaSolaLinea elementoCopiable">
                        clinicupbydb@gmail.com
                    </p>
                </div>
                <a href="https://www.google.com/maps/search/Calle+Federico+Geraldino,+Esquina+Dr+Jacinto+Ma%C3%B1on+%2313,+Edificio+D+Roca+Plaza,+Suite+204.+Ensanche+Para%C3%ADso/@18.4802671,-69.9412027,75m/data=!3m1!1e3?authuser=0&entry=ttu" target="_blank" class="col-sm-12 col-md-6 contenedorFlexible mt-3">
                    <div class="w-25 centrado">
                        <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/logos_empresas_de_terceros/ubicacion.png" alt="Icono ubicación" draggable="false">
                        <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/logos_empresas_de_terceros/ubicacion.png" alt="Icono ubicación" draggable="false">
                    </div>
                   <p class="h2 text-primary w-75 enUnaSolaLinea elementoCopiable">
                        Calle Federico Geraldino, Esquina Dr Jacinto Mañon #13, Edificio D Roca Plaza, Suite 204. Ensanche Paraíso.
                    </p>
                </a>
            </div>
        </div>

        
    </section>
    <footer class="bg-primary text-end" style="height: auto;">
        <a href="https://www.instagram.com/clinic.up.bydb/" target="_blank">
            <img src="/media/imagenes/logos_empresas_de_terceros/instagram_0.png" alt="Logo de Instagram" width="50vw" height="50vh" draggable="false">
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
    .tituloSeccion
    {
        display:flex;
        justify-content: center;
    }
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
    .enUnaSolaLinea
    {
        white-space: nowrap;            /* Mantiene el texto en una sola línea */
        overflow-x: auto;               /* Habilita la barra de desplazamiento horizontal si es necesario */
        /*width: 300vw;*/               /* Ajusta el ancho del contenedor */
        /*border: 1vw solid #ccc;*/     /* Opcional: Añade un borde para ver el área del contenedor */
        /*padding: 5vw;*/               /* Opcional: Añade un poco de padding */
    }
    .elementoCopiable
    {
        user-select: all;
    }
</style>