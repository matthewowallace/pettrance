<template>
  <div class="petg">
      <div class="uk-navbar-center pett">
          <h3>PetTrance</h3>
          <p>Pet Trap project</p>
      </div>
      <div uk-sticky="sel-target: .uk-navbar-container; cls-active: uk-navbar-sticky; bottom: #transparent-sticky-navbar">
          <nav class="uk-navbar-container" uk-navbar>
              <div class="uk-navbar-right">
                  <ul class="uk-navbar-nav">
                      <li>
                          <a href="#">Parent</a>
                      </li>
                      <li><a href="#">Item</a></li>
                  </ul>

              </div>
          </nav>
      </div>
   <!--<div class="hero-img">
     <img data-src="petlogo.png" alt="" uk-img uk-parallax="opacity: 1,1; y: -300,-300; x: -150,-150; scale: 0.5,0.5; viewport: 0.5;" >
     <img data-src="pets-6.png" width="1800" height="1200" alt="" uk-img id="layer2" >
   </div> -->
    <div class="calltoAction">
        <span>
            <button class="uk-button uk-button-default btn-icon">Get Started </button>
            <button class="uk-button uk-button-default btn-icon"><img src="../assets/cat.svg"  width="25px" height="auto"  /></button>
        </span>
    </div>

    <div id="modal-example" uk-modal>
      <div class="uk-modal-dialog uk-modal-body">
        <img src="../assets/pets-8.jpg">
        <h2 class="uk-modal-title">Dont leave us hanging subscribe for more</h2>
        <p>Subscribe to our newsletter to receive the latest updates and promotions.</p>
        <form class="uk-text-center">
          <div class="uk-margin">
            <div class="uk-inline">
              <span class="uk-form-icon uk-form-icon-flip"  uk-icon="icon: mail"></span>
              <input class="uk-input" type="text" placeholder="Enter e-mail...">
            </div>
          </div>
        </form>

        <p class="uk-text-center sub-btn">
          <button class="uk-button uk-button-default uk-modal-close" type="button">SUBSCRIBE</button>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
  import UIkit from 'uikit';

  export default {

  }

 /* UIkit.notification({
      "message": '<img src="../assets/cat.svg"/>',
      "status": 'primary',
      "pos": 'bottom-left',
      "timeout": '80000'
  }); */

  var util = UIkit.util;
  util.on(document, 'DOMContentLoaded', function () {
    var modalEl = util.$('#modal-example');
    UIkit.modal(modalEl).show();
  });
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

ul {
  list-style-type: none;
  padding: 0;
    margin: 0px;
}
li {
  display: block;
}
a {
  color: #42b983;
}

 .title{
   margin-left: 15%;
   margin-right: 15%;
   background-color: #ffffff;
   padding-top: 15px;
   padding-bottom: 15px;
 }


  .petg{
    background-image: url("../assets/2.jpg");
    background-size: cover;
    height: 100vh;
      position: relative;
  }

.uk-modal-body{
  width: 400px;
  padding: 0px;
}

.uk-modal-title{
  text-align: center;
  margin-top: 7px;
  font-weight: 500;
}

.uk-modal-body p{
  text-align: center;
  padding: 5px;
}

.sub-btn button{
  margin-top: -13px;
  width: 240px;
  background-color: rgba(50,0,0,0.5);
  color: #fff;
  margin-bottom: 20px;
}
  .hero-img{
    position: relative;
    overflow: hidden;
    width: 100%;
    height: 100vh;
  }

  .hero-img #layer1{
    position: absolute;
    transform: translateX(0);
    left: 0;
    height: auto;
  }

.hero-img #layer2{
  position: absolute;
  left: 0;
  top:0;
  transform: translateX(0);
  height: auto;
}

  .calltoAction{
    position: relative;
    top: 70%;
  }

.uk-navbar-nav{
    display: block;
}

.uk-navbar h3{
    color:#fff;
    font-family: Oxanium;
}
.uk-navbar-container:not(.uk-navbar-transparent){
    background-color: transparent;
    top:30px;
}
.uk-navbar-nav>li>a{
    min-height: 30px;
    color:#fff;
    font-family: Oxanium;

}

 .uk-navbar-nav>li>a.uk-open, .uk-navbar-nav>li>a:focus{
     color:#eee;
     text-decoration: line-through;
     margin-right: 50px;
     padding-right:30px;
     padding-left: 30px;

}

@keyframes borderglow{
    0%{ border: 1px solid rgba(255, 255, 255,0.8);}
    50% { border: 1px solid rgba(0, 229, 255,0.8); box-shadow: inset 0 0 40px rgba(0, 229, 255,1);}
    100% { border: 1px solid rgba(242, 64, 48, 0.829);}

}
.pett h3{
    position: relative;
    font-size: 8em;
    color: white;
    font-family: 'Oxanium';
}
    .pett p{
        color:white;
        text-decoration: line-through;
    }
   .calltoAction span button{
        margin-left: 5px;
    }

    .btn-icon{
        background-color: rgba(50,0,0,0.5);
        color: white;
    }

    .uk-notification-message img{
        width: 100px;
        height: 100px;
        display: inherit;
    }

  .uk-notification-bottom-center, .uk-notification-bottom-left, .uk-notification-bottom-right {
      top: auto;
      bottom: 170px;
  }

</style>
