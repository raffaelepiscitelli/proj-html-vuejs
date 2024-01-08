<template>
    <header>

        <section class="up-header">

            <div class="up-header-container flex">

                <img src="../assets/imgs/finance_logo_1x.png" alt="">

                <ul class="ul-header flex">

                    <HeaderMenu v-for="headerElement in headerMenu" :linkHeader="headerElement.link"/>

                </ul>

            </div>

        </section>

        <section class="jumbo">

            <div class="jumbo-container flex">

                <p>Right People. Right Investments.</p>

            </div>

        </section>

        <section class="bottom-header">

            <div class="bottom-header-container flex">

                <img src="../assets/imgs/client-logo-7-200x87.png" alt="">

                <img src="../assets/imgs/client-logo-8-200x87.png" alt="">

                <img src="../assets/imgs/client-logo-9-200x87.png" alt="">

                <img src="../assets/imgs/client-logo-5-200x87.png" alt="">

                <img src="../assets/imgs/client-logo-6-200x87.png" alt="">

                <img src="../assets/imgs/client-logo-7-200x87.png" alt="">

            </div>

        </section>
        
    </header>
</template>

<script>
import HeaderMenu from './HeaderMenu.vue';
export default {
    data() {
        return {
            headerMenu: [
                {
                    id: 1,
                    link: "Home"
                },
                {
                    id: 2,
                    link: "About"
                },
                {
                    id: 3,
                    link: "Services"
                },
                {
                    id: 4,
                    link: "Packages"
                },
                {
                    id: 5,
                    link: "Insight"
                },
                {
                    id: 6,
                    link: "Contact"
                },
                {
                    id: 7,
                    link: "+"
                }
            ]
        }
    },
    components: {
        HeaderMenu
    }
}
</script>

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;
</style>