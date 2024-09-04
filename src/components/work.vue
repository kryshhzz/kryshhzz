<script setup>

</script>

<template>
        <div class="work-bowl">
                <div class="work-cont stiff">
                        <div class="work-box wb2" >
                                <h2 id='mywork'>My Work</h2>
                        </div>
                        <div class="work-box wb1" onclick="window.location='https://veilmsg.pythonanywhere.com'">
                                <p>An open-source web platform for anonymous feedback && quesitons.</p>
                                <p>Tech: Django, Html, CSS, JS</p>
                                <b>Veilmsg</b>
                        </div>
                        <div class="work-box wb4" onclick="window.location='https://github.com/neonify/lessgo/'">
                                <p>A very fast url fuzzer in Golang used for pentesting.</p>
                                <p>Tech: Golang</p>
                                <b>Lessgo</b>
                        </div>
                        <div class="work-box wb5" onclick="window.location='https://Swing.pythonanywhere.com'">
                                <p>An online music streaming web platform.</p>
                                <p>Tech: Django, Html, CSS, JS, Ajax</p>
                                <b>Swing</b>
                        </div>
                        <div class="work-box wb3" onclick="window.location='https://bugz.pythonanywhere.com'">
                                <p>A simple blog website explaining various programming errors.</p>
                                <p>Tech: Django, Html, CSS, JS</p>
                                <b>Bugz</b>
                        </div>
                </div>
        </div>
</template>

<style scoped lang="scss">
        @import "../assets/base.scss";

        .work-bowl {
                width : 100%;
                min-height : 100vh;
                padding : 5em 1em 5em 1em;

                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                gap : 2em;
        }

        .work-cont{
                max-width : 100%; 
                height : 100%;

                display: grid;
                grid-template-columns: 1fr ;
                place-items : center;
                grid-gap :     1em;
        }
        .work-box  {
                width : 100%;
                height : 100%;
                background-color: $charcoal;
                border-radius: 1em; 
                text-decoration: none;  
                padding : 1em 1em 1.5em 1em;
                border : .1em solid rgb(176 255 146 / 05%);
                cursor :pointer;
                transition: .2s;

                display : flex;
                flex-direction: column;
                justify-content: space-between;
                align-items :start;
                gap : 1em;

                position : relative;
        }
        .work-cont div:hover  {
                box-shadow: inset 0em -5em 5em rgb(255 255 255 / 05%);
        }
        .wb2 {
                //box-shadow : 0 0em 10em #1ff99050 ;
                //box-shadow : 0 -5em 10em $lblue ;
                //background : linear-gradient(to top, $green,transparent 50% );
                padding : 1em;


                h2 {
                        text-transform: capitalize;
                        color : $white;
                        position: relative;
                }

        }
        .wb2::after {
                content : url("../assets/images/star.svg");
                position : absolute;
                bottom : 1em;
                right: 1em;
                width : 3em;
                height : 3em;
        }

        .work-box p {
                color : $gray;
                font-size : .9em;
                line-height : 1.5em;
        }
        .work-box b {
                color : $green;
                font-weight : 300;
                font-family: inherit;
                text-transform: capitalize;
                border-radius: .9em;
                font-size: 1.1em;
                margin-top : 2em;
                text-decoration: underline;
                text-decoration-thickness: .05em;
                text-underline-offset: .5em;
                text-decoration-color: $gray;
                text-decoration-style: wavy;
        }

        @media ( min-width : 730px){
                .work-cont{
                        width : 100%; 
                        height : 100%;

                        display: grid;
                        grid-template-columns: 1fr 1fr 1fr;
                        grid-template-rows : 1fr 1fr ;
                        place-items : center;
                        grid-gap : .75em;
                }
                .work-box {
                        width : 100%;
                        height : 100%;
                }

                .wb1 {
                        grid-column: 1/2;
                        grid-row : 1/2;
                }
                .wb2 {
                        grid-column: 2/3;
                        grid-row : 1/3;
                }
                .wb3 {
                        grid-column: 3/4;
                        grid-row : 1/2;
                }
                .wb4 {
                        grid-column: 1/2;
                        grid-row : 2/3;
                }
                .wb5 {
                        grid-column: 3/4;
                        grid-row : 2/3;
                }  
        }
        
</style>