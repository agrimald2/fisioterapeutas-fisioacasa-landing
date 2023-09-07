<template>
    <section class="testimonial-area pt-100 fix section" id="review" :style="bgImg">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="section-title text-center">
                        <div class="title-icon"></div>
                        <h2 class="title text-white">NUESTRO PROCESO</h2>
                        <p style="color: black;">
                            Empieza a recibir a tus clientes en <strong style="text-decoration: underline;"> 3 simples pasos</strong>
                        </p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <carousel class="testimonial-active owl-dot-style"
                        :items = "1"
                        :nav = "true"
                        :smartSpeed = "1000"
                        :navText = "['<','>']"
                    >
                        <!-- testimonial item start -->
                        <div v-for="(client, clients) in clients" :key="clients" class="testimonial-item">
                            <div class="testimonial-thumb">
                                <img :src="client.clientThumb" alt="client thumb">
                            </div>
                            <div class="testimonial-content">
                                <h6 class="client"><span style="font-family: fantasy">{{client.admirationS}}</span> {{ client.name }} <span style="font-family: fantasy">{{client.admirationE}}</span> <br> <span>{{ client.designation }}</span></h6>
                                <p class="desc">{{ client.desc }}</p>
                            </div>
                        </div>
                        <!-- testimonial item end -->
                    </carousel>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
    .title{
        color: #ED6C14!important;
    }
    .client{
        color: black;
        font-size: 1.3rem;
    }
    .desc{
        color: black;
        font-size: 1.1rem;
    }
</style>
<script>
import carousel from 'vue-owl-carousel'
export default {
    name: 'Testimonial',
    components: { 
        carousel 
    },
    data (){
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/blob-bg.png')})`
            },
            clients: [
                {
                    clientThumb: require("../assets/img/testimonial/1.png"), 
                    name: "REGISTRO", 
                    designation: "Crea tu cuenta como profesional", 
                    desc: "Llena el formulario de pre-registro para estar un paso más cerca de ser parte de nuestra comunidad de fisioterapeutas."
                },
                {
                    clientThumb: require("../assets/img/testimonial/2.png"), 
                    name: "HORARIOS y ZONA DE TRABAJO", 
                    designation: "Tienes la libertad de elegir", 
                    desc: "Podrás crear tus horarios en base a tu disponibilidad semanal y seleccionar las zonas en el mapa donde deseas trabajar dentro de tu panel de Fisioterapeuta."
                },
                {
                    clientThumb: require("../assets/img/testimonial/3.png"), 
                    name: "INGRESA TU TARIFA", 
                    designation: "Decide cuanto quieres ganar", 
                    desc: "Escoge tus precios por consulta, crea paquetes, promociones, ofertas, cobra por internet y más..."
                },
                {
                    clientThumb: require("../assets/img/testimonial/4.png"), 
                    admirationS: "¡",
                    admirationE: "!",
                    name: "Y LISTO", 
                    designation: "Ya puedes conseguir nuevos pacientes", 
                    desc: ""
                },
            ]
        }
    }
}
</script>

<style lang='scss'>
    @import '../assets/scss/variables.scss';
    @import '../assets/scss/components/testimonial.scss';
</style>
