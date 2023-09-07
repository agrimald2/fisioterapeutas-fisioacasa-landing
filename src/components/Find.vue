<template>
    <section class="features-area fix feature-style-3 bg-cover section" :style="bgImg" id="feature">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-7 col-md-6 order-2 order-md-1">
                    <div class="feature-thumb pt-30">
                        <img src="../assets/img/peoplePhone.png" alt="feature thumb">
                    </div>
                </div>
                <div class="col-lg-5 col-md-6 order-1 order-md-2">
                    <div class="section-title title-style-2 text-right pb-0">
                        <h2 class="title">DEJA QUE TUS PACIENTES TE ENCUENTREN</h2>
                        <p class="paragraph">
                            Tu crecimiento es nuestro compromiso, somos un equipo multidisciplinario que te brinda herramientas para que explotes tu potencial y logres tus metas.
                        </p>
                        <br>
                        <a href="https://fisioacasa.pe/fisio/register" class="read-more round-gradient">Regístrate</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
    .title{
        color:#ED6C14
    }
    .paragraph{
        color: #362d2d !important;
    }
    .read-more{
        background-color: #ED6C14;
    }
    img{
        border-radius: 5%;
    }
</style>
<script>
export default {
    name: 'Features',
    components: {
    },
    data () {
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/bg/blob-scene.png')})`
            }
        }
    }
}
</script>

<style lang='scss'>
    @import '../assets/scss/variables.scss';
    @import '../assets/scss/components/feature.scss';
</style>
