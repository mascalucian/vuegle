<template>
    <div id="footer-" class="botflex botflex-1"> 
        <div id="footer-" class="botstanga footer- footer-s-1">
            <a href="#" id="despre">
                Despre
            </a>
            <a href="#" id="advertising">
                Publicitate
            </a>
            <a href="#" id="business">
                Companii
            </a>
            <a href="#" id="hsw">
                Cum funcționează Căutarea
            </a>
        </div>
        <div id="footer-" class="botdreapta footer- footer-s-2">
            <a href="#" id="privacy">Confidențialitate</a>
            <a href="#" id="terms">Termeni</a>
            <a href="#" id="settings">Setări</a>
        </div>
    </div>
     <div id="footer2-" class="botflex2 botflex2-1 footer2-1">
        <div> <a href="#" id="tara" class="botstanga">România</a></div>
    </div> 
</template>

<script>
export default {
    setup() {
        
    },
}
</script>

<style scoped>

.botflex {
    position: absolute;
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    width: 99%;
    bottom: 0;
    height:250px;
}
.botflex2 {
    position: absolute;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    width: 99%;
    bottom: 50px;  
    height: 50px;
    background-color: rgba(0,0,0,.05);
    color: rgba(0,0,0,.54);
}
.botstanga {
    display: flex;
    justify-content: flex-start;
    width: 50%;
    padding-left: 10px;
}
.botdreapta { 
    display: flex;
    justify-content: flex-end;
    width: 50%;
    padding-right: 20px;
}
@media only screen and (max-width: 1000px) {
    .footer-s-1 {min-width: 100%;justify-content: center;position: absolute;}
    .footer-s-2 {min-width: 100%;justify-content: center;position: absolute;left: 0;}
}
@media only screen and (max-width: 1000px) {
    .botflex2-1 {bottom:100px;}
}
@media only screen and (max-width: 1000px) {
    .botflex-1 {flex-direction: column;justify-content: flex-end;}
}
.footer- {
    position: relative;
    bottom: 0;
    height: 50px;
    background-color: rgba(0,0,0,.05);
    color: rgba(0,0,0,.54);
    width: 50%;
}
.footer2- {
    position: absolute;
    bottom: 50px;
    height: 50px;
    background-color: rgba(0,0,0,.05);
    width: 98vw;
    color: rgba(0,0,0,.54);
    
    border-bottom: 1px solid #dadce0;
    font-size: 14px;
    color: rgba(0,0,0,.54);
}
#advertising,#despre,#business,#hsw,#privacy,#terms,#settings,#tara {
    justify-self: center;
    align-self: center;
    color: #70757a;
    font-size: 14px;
    padding: 10px;
    text-decoration: none;
}
#tara {
    font-size: 15px;
    margin-left:15%;
}
</style>