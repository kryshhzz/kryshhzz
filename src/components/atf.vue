<script setup>

        import {ref, onMounted} from 'vue';

        const words = ["Krishna Prasad","Building Webapps", "Always Learning"];
        const word = ref("")
        var i = ref(0)

        function change(){
                word.value.innerHTML = words[Math.floor(Math.random() * words.length)];
        }
        onMounted( ()=>{
                setInterval(function (){
                        if (i.value < words.length-1) i.value++
                        else i.value = 0
                }, 3000);
        })
</script>

<template>
        <div class="atf">
                <div class="atf-container stiff">  
                        <div class="layer">
                                <h1>{{words[i]}}</h1>
                                <p>
                                       Namaskaram ! I’m Krishna Prasad, an MCA student at NIT Warangal, mastering the art of full-stack development to deliver exceptional web experiences.
                                </p>
                                <div class="cta">
                                        <a href='#mywork'>View My Work</a>
                                </div>
                        </div>
                        <div class="bg-img">
                                <img src="../assets/images/avatar.png" alt="">
                        </div>
                </div>
        </div>
</template>

<style lang="scss">

        @import "../assets/base.scss";
        @import url('https://fonts.googleapis.com/css2?family=Yellowtail&display=swap');

        .atf {
                //background : linear-gradient(to top,black,#303030);
                background : linear-gradient(to top,rgba(255 255 255 / 13%), black);
                width : 100%;
        }
        .atf-container {
                width : 100%;
                height : 100vh;

                display : flex;
                // flex-direction: column;
                justify-content : center;
                align-items: center;

                position: relative;
        }

        .layer {
                width : 100%;
                padding : 4em 1.5em 11em 1.5em;
                color : $white;

                display : flex;
                flex-direction : column;
                justify-content : center;
                align-items: center;
                gap : 3em;
        }
        .layer h1 {
                text-align : center;
                text-transform: capitalize;
                font-size: clamp(2rem, 2vw + 1rem, 4rem); 

                position: relative;
                animation: fade 3s infinite;
        }
        @keyframes fade {
                0% {
                        opacity : 0;
                }
                10% {
                        opacity: 100%;
                }
                90% {
                        opacity : 100%;
                }
                100% {
                        opacity: 0;
                }
        }
        .layer h1::before {
                content : "char *kryshhzz";
                // font-family: "Yellowtail" , cursive;
                position : absolute;
                top : -2em;
                left : 50%; 
                font-size :.45em;
                transform: translateX(-50%);
                text-transform: none;
                color : $green;
                font-weight: 300;
                font-style : italic;
        }
        // .layer h1::after {
        //         content : url('../assets/images/arrow.svg');
        //         width : 1.1em;
        //         position : absolute;
        //         top : -1.1em;
        //         left : 73%;
        //         transform: scaleX(-1) rotate(130deg);
        // }
        .layer p {
                text-align : center;
                line-height: 1.75em;
                font-weight: 300;
                color : $gray;
        }

        .cta {
                padding : 1em 1em 0em 1em;
        }
        .cta a{
                background : $white;
                color : $black;
                border : none;
                padding : .8em 2em;
                outline : none;
                text-transform: uppercase;
                font-family: $base-font;
                border-radius: 100em;
                font-weight : 800;
                font-size: .9em;
                transition: .25s;
                cursor : pointer;
                box-shadow: 0 0 10em $black;
                text-decoration: none;
        }
        .cta a:hover{
                box-shadow: 0 0 20em $green;
        }
        .atf-container .bg-img {
                max-width : 14em;
                
                display : flex;
                flex-direction: column;
                justify-content: flex-end;
                align-items : center;
        
                position : absolute;
                bottom : 0;
        }
        .bg-img::after {
                content : 'Dedicated';
                position : absolute;
                bottom : 4em;
                left : -2em;
                background: rgba(255,255,255,.22);
                border : .1em solid rgba(255,255,255,.2);
                padding : .45em 1.25em;
                font-size : .8em;

                transform : rotate(15deg);

                border-radius: 100em;
                color : $white;
                z-index : 4;
        }
        .bg-img::before {
                content : 'Innovative';
                position : absolute;
                top : 1em;
                right : -2.5em;
                background: rgba(255,255,255,.22);
                border : .1em solid rgba(255,255,255,.2);
                padding : .45em 1.25em;
                font-size : .8em;
                transform : rotate(-10deg);
                border-radius: 100em;
                color : $white;
                z-index : 2;
        }
        .atf-container .bg-img img {
                width : 100%;
                position : relative;
                z-index : 3;
        }

</style>