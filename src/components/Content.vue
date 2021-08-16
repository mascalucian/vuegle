<template>
    <div id="main">
        <div id="logo"><img src="../assets/logo1.png"></div>
            <div id="search" class="searchbox">
                <img src="../assets/lens.png" class="lens">
                <input type="text" class="searchtext">
                <img src="../assets/keyb.png" class="keyb">
                <img src="../assets/mic.png" class="mic">  
            </div>
            <div id="flexbox">
            <button id="google-search-btn">Căutare Google</button><button id="random-search-btn">Mă simt norocos</button>
        </div>
        <p id="google-text">
            Google oferit în:
            <a href="#" id="limba" class="spatiu">
                English
            </a>
            <a margin-left="5px" href="#" id="limba" class="spatiu">
                Magyar
            </a>
            <a href="#" id="limba" class="spatiu">
                Deutsch
            </a>
        </p>
    </div>
</template>

<script>
export default {
    setup() {
        
    },
}
</script>

<style scoped>
#main {
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
    align-items: center;
    margin-top: 200px;
    margin-left:auto;
    margin-right:auto;
    min-width: 400px;
    height: 300px;
    width: 50%;
}
.lens {
    max-width: 14px;
    margin-left: 15px;
    margin-top: 10px;
    height: 15px;  
}
.searchbox {
    display: flex;
    padding: 5px 8px 0 16px;
    padding-left: 14px;
    width: 60%;
}
.searchtext {
    margin-left: 20px;
    width: 80%;
    height: 20px;
    border: none; 
    margin-top: 5px;
}
.searchtext:focus {
    outline: none;
}
.keyb {
    max-width: 20px;
    height: 20px;
    margin-top: 8px;
    margin-left: 17px;
    opacity: 60%;
    padding-left: 160px;
}
.mic {
    max-width: 13px;
    height: 20px;
    margin-left: 20px;
    margin-top: 10px;
    padding-right: 20px;
}
#search {
    height: 44px;
    min-width: 400px;
    align-self: center;
    justify-self: center;
    border: 1px solid rgba(0, 0, 0, 0.151);
    border-radius: 30px;
    margin-top: 21px;
    
}
#search:focus {
    box-shadow: 1px 1px 5px grey;
    
}
#search:hover {
    box-shadow: 1px 1px 5px rgba(128, 128, 128, 0.585);
}
#flexbox {
    display: flexbox;
    grid-area: flexbox;
    justify-self: center;
    align-self: center;
    margin-top: 22px;
}
#google-search-btn {
    border: none;
    font-size: 14px;
    color: #3c4043;
    margin-right: 16px;
    padding: 9px 15px 9px 15px;
    border-radius: 3px;
    background-color: #f8f9fa;
    
}
#random-search-btn {
    border: none;
    font-size: 14px;
    color: #3c4043;
    padding: 9px 15px 9px 15px;
    border-radius: 3px;
    background-color: #f8f9fa;
}
#google-search-btn:hover {
    border: 1px solid rgba(0, 0, 0, 0.226);
}
#random-search-btn:hover {
    border: 1px solid rgba(0, 0, 0, 0.226);
}
#google-search-btn:focus {
    border: 1px solid #4285f4;
}
#random-search-btn:focus {
    border: 1px solid #4285f4;
}
.spatiu {
    margin-left: 6px;
}
#google-text {
    grid-area: google-text;
    justify-self: center;
    margin-top: 23px;
    margin-left: -2px;
    font-size: 13px;  
}
#limba {
    color: #1a0dab;
    font-size: 13px;
    text-decoration: none;
}
</style>