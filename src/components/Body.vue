<template>
    <div>
        <div class="uk-flex uk-flex-center sec-1">
            <div class="uk-card uk-card-default uk-card-body" uk-parallax="opacity: 0,1; x: -200,0; viewport: 0.5">
                <img src="../assets/rabbit.svg" width="40px" height="auto">
                <h3>Walking</h3>
                <p>  The grid system of UIkit follows the mobile-first approach and accomodates up to 10 grid columns.
                    It uses units with predefined classes inside each grid, which define the column width.
                    It is also possible to combine the grid with classes from the Flex component, although it work
                </p>
                <button class="uk-button uk-button-default btn-icon">Get Started </button>
            </div>
            <div class="uk-card uk-card-default uk-card-body uk-margin-left" uk-parallax="opacity: 0,1; y: 200,0; viewport: 0.5">
                <img src="../assets/khao-manee-cat.svg" width="40px" height="auto">
                <h3>Walking</h3>
                <p>  The grid system of UIkit follows the mobile-first approach and accomodates up to 10 grid columns.
                    It uses units with predefined classes inside each grid, which define the column width.
                    It is also possible to combine the grid with classes from the Flex component, although it work
                </p>
                <button class="uk-button uk-button-default btn-icon">Get Started </button>
            </div>
            <div class="uk-card uk-card-default uk-card-body uk-margin-left" uk-parallax="opacity: 0,1; y: 600,0; viewport: 0.5">
                <img src="../assets/footprint.svg" width="40px" height="auto">
                <h3>Walking</h3>
                <p>  The grid system of UIkit follows the mobile-first approach and accomodates up to 10 grid columns.
                    It uses units with predefined classes inside each grid, which define the column width.
                    It is also possible to combine the grid with classes from the Flex component, although it work
                </p>
                <button class="uk-button uk-button-default btn-icon">Get Started </button>
            </div>
        </div>

        <div class="uk-grid p-1" uk-parallax="opacity: 0.5,1; y: 0,10; viewport: 0.5">
                    <div class="uk-width-1-2 side-img"></div>
                    <div class="uk-width-1-2  para-1" >
                            <h3> Getting Started</h3>
                            <p>
                                The grid system of UIkit follows the mobile-first approach and accomodates up to 10 grid columns.
                                It uses units with predefined classes inside each grid, which define the column width.
                                It is also possible to combine the grid with classes from the Flex component, although it works only in modern browsers
                            </p>
                    </div>
        </div>
        <div class="uk-grid p-1" uk-parallax="opacity: 0.5,1; y: 0,10; viewport: 0.5">
            <div class="uk-width-1-2  para-1" >
                <h3> Getting Started</h3>
                <p>
                    The grid system of UIkit follows the mobile-first approach and accomodates up to 10 grid columns.
                    It uses units with predefined classes inside each grid, which define the column width.
                    It is also possible to combine the grid with classes from the Flex component, although it works only in modern browsers
                </p>
            </div>
            <div class="uk-width-1-2 side-img-2"></div>
        </div>
        <div class="to-top"><a href="#"  uk-scroll> TO TOP</a></div>
        <div class="vid">
            <iframe width="100%" height="720" src="https://www.youtube.com/embed/e14xmWKFgEc" uk-video="autoplay: inview" frameborder="0"  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>

    .para-1{
        height: 400px;
        overflow: hidden;
    }

    .para-1 h3{
        margin-top: 10%;
    }

    .para-1 p{
        padding: 20px 50px;

    }

    @media (min-width: 1200px) {
        .uk-grid > * {
            padding-left: 0px;
        }
    }

    .side-img{
        background-image: url("../assets/4.png");
        background-size: cover;
        background-attachment: fixed;
        background-repeat: no-repeat;
        background-position: -430px -200px;
    }
    .side-img-2{
        background-image: url("../assets/5.png");
        background-size: cover;
        background-attachment: fixed;
        background-repeat: no-repeat;
        background-position: 430px -250px;
    }


    .sec-1{
        margin: 50px 0;
    }

    .btn-icon{
        background-color: rgba(50,0,0,0.5);
        color: white;
    }

    .uk-card-default {
        background: #fff;
        color: #666;
        box-shadow: 0 0px 0px rgba(0,0,0,.08);
        transition-duration: 1s;
    }

    .uk-card-default:hover {
        background: #fff;
        color: #666;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }

    @media (min-width: 1200px) {
        * + .uk-grid-margin, .uk-grid + .uk-grid, .uk-grid > .uk-grid-margin {
            margin-top: 0px;
        }
    }


    .to-top{
        background-color: rgba(50,0,0,0.7);
        font-family: Oxanium,sans-serif;
        color: white;
        position: fixed;
        top: 80%;
        left: 92%;
        height: 20px;
        padding: 20px 5px;
        box-shadow: -2px -2px 52px rgba(255,255,255,0.2),
                    2px 2px 5px rgba(0,0,0,0.1),
                    inset -2px -2px 2px rgba(255,255,255,0.2),
                    inset 2px 2px 2px rgba(255,255,255,0.6);
    }

    .to-top a{
        color: #fff;
    }

    .to-top a:hover{
        text-decoration: line-through;
    }
    .vid{
        margin-top: 10px;
    }

</style>