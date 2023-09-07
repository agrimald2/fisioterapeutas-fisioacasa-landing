<template>
    <footer>
        <div class="footer-main dark-bg section-padding" :class="FooterStyle">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="footer-content text-center">
                            <ul class="footer-social-link">
                                <li v-for="(social, socials) in socials" :key="socials">
                                    <a :href="social.link"><i :class=social.icon></i></a>
                                </li>
                            </ul>
                            <h3 class="footer-title">¡SE PARTE DE FISIOACASA!</h3>
                            <p>La plataforma innovadora hecha para ti...</p>
                            <a href="https://fisioacasa.pe/fisio/register"
                                class="read-more round-gradient mt-3">Regístrate</a>
                            <p class="mt-4" style="font-size:0.8rem">
                                Toda la información recopilada de los profesionales postulantes a formar parte de la
                                comunidad de Fisioacasa.pe es de carácter confidencial y para uso privado de FISIOACASA
                                PERU
                                SAC.
                            </p>
                            <p class="cursor-pointer mt-4 mb-4" style="font-size: 0.8rem">
                                Respaldados por el <a
                                    href="https://cri-ctmp.org.pe/tramites-servicios/habilidad-profesional/"
                                    target="_blank"> Colegio
                                    de Tecnólogos Médico del Perú</a>
                                <img class="ml-2" src="../assets/img/logoCTMP.png" height="50px" width="auto">
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom black-bg" :class="FooterStyle">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 order-2 order-md-1">
                        <div class="copyright">
                            <p>&copy; 2022 <b class="text-white">FISIOACASA PERU</b> SAC por <a
                                    href="https://e-pask.com/"><b>e-Pask</b></a></p>
                        </div>
                    </div>
                    <div class="col-md-6 order-1 order-md-2">
                        <div class="useful-link">
                            <a href="#">Home</a>
                            <a href="#">Regístrate</a>
                            <a href="#">Inicia Sesión</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: ["FooterStyle"],
    data() {
        return {
            socials: [
                { icon: "fa fa-facebook", link: "https://www.facebook.com/Fisioacasa.pe?paipv=0&eav=Afak4gwVeMeIkyV45iA_Y9LzuQPg82UPWBgzMqAC4Oa0r8G5W373mmdav_yMV1FTfec" },
                { icon: "fa fa-instagram", link: "https://instagram.com/fisiacasa.pe" },
                { icon: "fa fa-whatsapp", link: "https://wa.me/51990648927" },
                //{ icon: "fa fa-linkedin", link: "https://www.linkedin.com/company/76152586/admin/" },
            ]
        }
    }
}
</script>

<style lang='scss'>
@import '../assets/scss/variables.scss';
@import '../assets/scss/components/footer.scss';</style>
