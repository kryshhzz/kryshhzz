<script setup>
        import Header from '../components/header.vue'
        import atf from '../components/atf.vue'
        import Work from '../components/work.vue'
        import Footer from '../components/footer.vue'
        import About from '../components/about.vue'
</script>

<template>
        <Header />
        <atf />
                <div class="line">
                        <div>
                                <p>Django</p>
                                <p>HTML</p>
                                <p>CSS</p>
                                <p>JavaScript</p>
                                <p>VueJS</p>
                                <p>Python</p>
                                <p>Go</p>
                                <p>Linux</p>
                                <p>SEO</p>

                                <p>Django</p>
                                <p>HTML</p>
                                <p>CSS</p>
                                <p>JavaScript</p>
                                <p>VueJS</p>
                                <p>Python</p>
                                <p>Go</p>
                                <p>Linux</p>
                                <p>SEO</p>
                        </div>
                </div>
        <Work />
        <About />
        <Footer/>
</template>

<style lang="scss" scoped>

        @import "../assets/base.scss";

        .line {
                width : 100%;
                background : $green;
                overflow-x : hidden;   
        }
        .line div {
                display : flex;
                justify-content : space-around;
                align-items : center;

                padding : 2em 0;
                width : 100%;
                animation : 20s marquee linear infinite;
        }
        .line p {
                padding : 0 5em;
                color : $black;
                text-transform : uppercase;
                letter-spacing : .1em;
                font-size : .8em;
                font-weight: 600;
                border-left : .1em dashed $charcoal;
        }

        @keyframes marquee {
                0%   { transform: translateX(0); }
                100% { transform: translateX(calc(-300px * 6)); }
        }

</style>