<template>
    <div id="parteadesus">
       
        <a href="#" id="gmail">{{gmail}}</a>
        <a href="#" id="image">{{image}}</a>
        <a href="#"><img id="menu" src="../assets/vectorpaint.svg" ></a>
        <a href="#" id="loggedin" class="popup"><img src="../assets/iconprof.png">
            <span class="popuptext" id="myPopup"><img src="../assets/popupopen.png"></span>
        </a>
    </div>
</template>

<script>
export default {
    
  name: 'Header',
  props: {
    gmail: String,
    image: String,
    dotsimg: String
  }
}
</script>

<style scoped>
    #parteadesus {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    margin: 0px 10px 0 10px;
    }
    #gmail {
    justify-self: center;
    align-self: center;
    margin-bottom: 7px;
    margin-right: 2px;
    margin-left: 17px;
    font: 13px/27px Roboto,RobotoDraft,Arial,sans-serif;
    text-decoration: none;
    }
    #image {
        margin-right: 10px;
        margin-bottom: 7px;
        margin-left: 12px;
        font: 13px/27px Roboto,RobotoDraft,Arial,sans-serif;
        text-decoration: none;
    }
    #menu {
        margin-left: 20px;
        margin-bottom: 4px;
        height:16px; 
        width:16px;
    }
    #loggedin {
        margin-left: 20px;
        grid-area: sign-in;
        justify-self: center;
        align-self: center;
        margin-bottom: 2px;
    }
    /* Popup container */
.popup {
    position: relative;
    display: inline-block;
    cursor: pointer;
  }
  
  /* The actual popup (appears on top) */
  .popup .popuptext {
    visibility: hidden;
    width: 350px;
    height: 400px;
    background-color: #fff;
    color: #555;
    text-align: left;
    border-radius: 6px;
    padding: 8px 0;
    position: absolute;
    z-index: 1;
    top: 145%;
    right: 5%;
    margin-left: -80px;
    box-shadow: 1px 1px 5px grey;
  }
  
  
  
  /* Toggle this class when clicking on the popup container (hide and show the popup) */
  .popup .show {
    visibility: visible;
    -webkit-animation: fadeIn 1s;
    animation: fadeIn 1s
  }
  .gb_Ca {
    -webkit-background-size: 32px 32px;
    background-size: 32px 32px;
    border: 0;
    -webkit-border-radius: 50%;
    border-radius: 50%;
    display: block;
    margin: 0px;
    position: relative;
    height: 32px;
    width: 32px;
    z-index: 0;
}
.gb_Ca:hover, .gb_Ca:focus {
    -webkit-box-shadow: 0 1px 0 rgb(0 0 0 / 15%);
    box-shadow: 0 1px 0 rgb(0 0 0 / 15%);
}
  

  @-webkit-keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
  }
  
  @keyframes fadeIn {
    from {opacity: 0;}
    to {opacity:1 ;}
  }
  
</style>