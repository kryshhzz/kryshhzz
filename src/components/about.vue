<script>

</script>

<template>
        <div class="about-bowl">
                <div class="about-cont stiff">
                        <h2>whoami</h2>
                        <p>
                                <span class="italic">Hello!</span> I’m Krishna Prasad, pursuing my MCA at NIT Warangal, where I focus on full-stack development to build exceptional web applications. Known for my quick learning abilities and passion for coding, I have also worked as a freelancer on Fiverr, creating eye-catching landing pages.
                        </p>
                        <br>
                        <h2>codebase</h2>
                        <div class="skills-box">
                                <span>Python</span>
                                <span>Golang</span>
                                <span>C++</span>
                                <span>Django</span>
                                <span>VueJS</span>
                                <span>HTML</span>
                                <span>CSS</span>
                                <span>JavaScript</span>
                                <Span>Linux</Span>
                                <span>SEO</span>
                        </div>
                        
                </div>
                <div class="edu-cont stiff">
                        <h2>education</h2>
                        <div class="edu-box">
                                <a href="https://nitw.ac.in" target="_blank">National Insititue of Technology, Warangal</a>
                                <p>Master of Computer Applications</p>
                                <p>2024 - 2027</p>
                        </div>
                        <div class="edu-box">
                                <a href="https://ucssou.osmania.ac.in" target="_blank">University College of Science, Saifabad, Osmania Univeristy</a>
                                <p>Bachelor of Computer Applications</p>
                                <p>2021 - 2024</p>
                        </div>
                        <div class="edu-box">
                                <a href="https://hpsbegumpet.org.in">The Hyderabad Public School, Begumpet</a>
                                <p>Indian School Certificate</p>
                                <p>2019 - 2021</p>
                        </div>
                        <div class="edu-box">
                                <a href="https://hpsbegumpet.org.in">The Hyderabad Public School, Begumpet</a>
                                <p>Indian Certificate of Secondary Education</p>
                                <p>2009 - 2019</p>
                        </div>
                </div>
        </div>
</template>

<style lang="scss" scoped>
        @import "../assets/base.scss";

        .about-bowl {
                width : 100%;
                padding : 1em;

                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: start;
                gap : 3em;
        }
        .about-cont {
                width : 100%;
                //background : $charcoal;
                //border : .1em solid rgb(176 255 146 / 05%);
                padding : 2em 1em;
                color : $white;
                //border-radius: 1em;

                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: start;
                gap : 2em;
        }
        .about-cont h2 {
                
        }
        .about-cont p {
                color : $gray;
        }
        .skills-box {
                width : 100%;
                display : flex;
                flex-wrap: wrap;
                gap : 1em;
        }
        .skills-box span {
                color : $gray;
                background : $charcoal;
                padding : .5em 1em;
                border-radius: 100em;
                border :.075em solid rgb(255 255 255 / 5%);
        }
        .edu-cont {
                width : 100%;
                padding : 1em;

                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: start;
        }
        .edu-cont h2 {
                color : $white;
        }
        .edu-box {
                padding : 2em 3em;
                margin-left : 1em;
                position: relative;

                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: start;
                gap : .75em;
        }
        .edu-cont .edu-box:not(:last-child)::before {
                content : '';
                position : absolute;
                top : 2em;
                height : 100%;
                left : 0;
                border-left : .15em solid rgb(176 255 146 / 10%);
        }
        .edu-box::after {
                content : '';
                position : absolute;
                top : 2em;
                bottom : 0;
                left : 0;
                transform: translate(-45%);
                width : 1em;
                height: 1em;
                border-radius: 50%;
                background : $black;
                box-shadow : 0 0 .5em $green;
        }
        .edu-box a {
                color : $green;
                font-weight : 400;
                text-decoration: none;
        }
        .edu-box p {
                color : $gray;
        }
</style>