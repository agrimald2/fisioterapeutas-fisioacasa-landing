<template>
    <section class="about-app-store" id="us">
        <div class="container-fluid p-0">
            <div class="row no-gutters">
                <div class="col-lg-6">
                    <div class="about-app section-padding bg-cover" :style="bgImg">
                        <div class="section-title title-style-4 text-center">
                            <h2 class="title">¿QUIENES SOMOS?</h2>
                            <p class="paragraph">
                                Somos un equipo multidisciplinario que te brinda herramientas para que explotes tu
                                potencial y logres tus metas.
                                <br>
                                - Tu crecimiento es nuestro compromiso -
                            </p>
                        </div>
                        <div class="about-app-content text-center">
                            <p>
                                <img src="../assets/fisiocasa/Logo/logo.png" alt="" srcset="">
                                <a href="" class="fisio_link">
                                    fisioacasa.pe
                                </a>
                                es una plataforma digital de servicios de
                                Terapia Física a domicilio
                                <br>
                                que brinda a sus pacientes la posibilidad de mantener su
                                bienestar con un equipo de profesionales calificados, colegiados y licenciados que
                                garantizan acompañarlos
                                <br>    
                                en su evolución durante su tratamiento.
                            </p>
                            <br>
                            <a href="https://fisioacasa.pe/fisio/register" class="read-more round-gradient">Regístrate</a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6">
                    <CounterUp />
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
img {
    height: 3.5vh;
    margin-bottom: 0.75rem;
    margin-right: 0.10rem;
}

.title {
    font-size: 30px !important;
}

.fisio_link {
    color: white;
    text-decoration-color: #ED6C14;
    font-weight: bolder;
    font-size: 1.1rem;
}

p {
    color: white !important;
}
</style>
<script>
import CounterUp from '../components/CounterUp'
export default {
    components: {
        CounterUp
    },
    data() {
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/bg/bgfi.png')})`
            }
        }
    }
}
</script>