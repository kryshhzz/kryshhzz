
<script setup>

</script>
<template>  
        <header>
                <div class="header stiff">
                        <div class="logo">kryshhzz</div>
                        <nav>
                                <p>Contact:</p>
                                <a href="https://www.linkedin.com/in/kryshhzz/">linkedin</a>
                                <a href="mailto:kryshhzz@protonmail.com">kryshhzz@protonmail.com</a>
                        </nav>
                </div>
        </header>
</template>

<style lang="scss" scoped>
        @import '../assets/base.scss';

        header {
                width : 100%;
                background : linear-gradient(to bottom, rgba(0,0,0,.75), transparent);
                padding : 2em 1em;

                position: fixed;
                top : 0;
                left : 0;
                z-index: 100;
        }
        .header {
                width : 100%;
                display :flex;
                justify-content : space-between;
                align-items: center;
                gap : 1em;
        }
        .header .logo {
                color : $white;
                font-weight : 700;
                font-size: 1em;
                text-transform: uppercase;
                letter-spacing: .25em;
        }
        .header nav {
                width : 100%;
                padding : 0 2em 0 0;
                display : flex;
                justify-content: flex-end;
                align-items: center;
                gap : 1em;

                font-size : .9em;
        }
        
        @media (max-width : 560px){
                .header {
                        width : 100%; 

                        display :flex;
                        flex-direction: column;
                        justify-content : center;
                        align-items: center;
                        gap : 1em;
                }
                .header nav {
                        width : 100%;
                        padding : 0;
                        display : flex;
                        justify-content: center;
                        align-items: center;
                        gap : 1em;
                }
        }
        .header p {
                color : $gray;
                text-transform: capitalize;
                font-size: .9em;
        }
        .header a {
                color : $white;
                text-decoration: none;
                font-weight: 300;
        }
        .header nav a:hover {
                color : $green;
        }

</style>