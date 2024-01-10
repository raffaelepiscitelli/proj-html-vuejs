<template>
    <footer>

        <div class="footer-container">

            <div class="up-footer flex">

                <div class="flex">

                    <img src="../assets/imgs/finance_logo_footer.png" alt="">

                </div>

                <div class="flex">

                    <span>Recent post</span>

                    <ul>

                        <FooterMenu v-for="footerElement in recentPost" :linkFooter="footerElement.link"/>

                    </ul>

                </div>

                <div class="flex">

                    <span>Services</span>

                    <ul>

                        <FooterMenu v-for="footerElement in services" :linkFooter="footerElement.link"/>

                    </ul>

                </div>

                <div class="flex">

                    <span>Latest</span>

                    <i class="fa-brands fa-twitter" style="color: #5aaeeb;"></i>

                </div>

            </div>

            <div class="bottom-footer flex">

                <div>

                    <span>&#169; Copyright 2012 - 2020 | Avada Theme by Theme Fusion | All Rights Reserved | Powered by WordPres</span>

                </div>

                <div>

                    <i class="fa-brands fa-facebook-f" style="color: #ffffff;"></i>

                    <i class="fa-brands fa-twitter" style="color: #ffffff;"></i>

                    <i class="fa-brands fa-youtube" style="color: #ffffff;"></i>

                    <i class="fa-brands fa-instagram" style="color: #ffffff;"></i>

                    <i class="fa-solid fa-angle-up" style="color: #d1d1d2;"></i>

                </div>

            </div>

        </div>

    </footer>
</template>
<script>
import FooterMenu from './FooterMenu.vue';
export default {
    data() {
        return {
            recentPost: [
                {
                    id: 1,
                    link: "> When is it the rigth time to sell your company?"
                },
                {
                    id: 2,
                    link: "> Personal debt or company debt we explore your options"
                },
                {
                    id: 3,
                    link: "> An interview with a so-called business angel"
                },
            ],
            services: [
                {
                    id: 1,
                    link: "> Small business loan services"
                },
                {
                    id: 2,
                    link: "> Credit rating advice services"
                },
                {
                    id: 3,
                    link: "> Crowd funding services"
                },
            ],
        }
    },
    components: {
        FooterMenu
    }
}
</script>
<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;
</style>