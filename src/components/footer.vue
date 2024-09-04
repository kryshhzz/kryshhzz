<script>

</script>

<template>
        <footer>
                <div class="footer stiff">
                        <h2>social()</h2>
                        <div class="links">
                                <a href="https://www.linkedin.com/in/kryshhzz/" target="_blank">linkedin</a>
                                <a href="mailto:kryshhzz@protonmail.com"target="_blank">email</a>
                                <a href="https://github.com/kryshhzz" target="_blank">github</a>
                                <a href="https://fiverr.com/kryshhzz" target="_blank">fiverr</a>
                                <a href="https://leetcode.com/u/ZVRnydgUcI/" target="_blank">leetcode</a>
                        </div>
                </div>
        </footer>
</template>

<style scoped lang="scss">
        @import "../assets/base.scss";

        footer {
                width : 100%;
                padding : 10em 1em 1em 1em;
                background : linear-gradient(to bottom, transparent, rgb(255 255 255 / 10%));
        }
        .footer {
                width : 100%;
                background : rgb( 0 0 0 / 30%);
                border : .05em solid rgb(255 255 255 / 10%);
                padding : 2em;
                border-radius: 1em;

                display : flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                gap : 2em;
        }
        .footer h2 {
                color : $green;
        }
        .footer .links {
                display : flex;
                justify-content: center;
                align-items: center;
                gap : 1em;
        }
        .links a {
                color : $gray;

                text-decoration: underline;
                text-decoration-thickness: .05em;
                text-underline-offset: .5em;
                text-decoration-color: $gray;
                text-decoration-style: wavy;
        }
        
</style>