<template>
    <div class="container-nav">
        <img src="./image-src/logo.png" alt="Logo" class="logo-image" />
        <NavButton buttonText="MAIN"></NavButton>
        <NavButton buttonText="PLAY"></NavButton>
        <NavButton buttonText="WINNERS"></NavButton>
        <NavButton buttonText="TOURNAMENTS"></NavButton>
        <NavButton buttonText="STREAMING"></NavButton>
        <NavButton buttonText="DEVOLOPERS"></NavButton>
        <NavButton buttonText="MARKET"></NavButton>
        <button class="download-app-button">
            Download app
        </button>
        <div class="container-profile-bar">
            <img src="./image-src/coin-nav.png" alt="Coin" class="coin-image" />
            <div class="column-coin">
                150.000
            </div>
            <img src="./image-src/money-nav.png" alt="Money" class="coin-image" />
            <div class="column-money">
                150.000
            </div>
            <div class="profile-icon">
                <img src="" alt="" class="profile-image" />
            </div>
        </div>
    </div>
</template>

<script>
import NavButton from './NavButton.vue';
export default {
    name: "Navigation",
    components: {
        NavButton,
    }
}
</script> 

<style>
html,
body {
    height: 100%;
    margin: 0;
}

.container-nav {
    width: 100%;
    height: 101px;
    background-color: #202936;
    display: flex;
    align-items: center;
}

.logo-image {
    margin-left: 3%;
}

.download-app-button {
    background-color: #0661dc;
    color: white;
    font-size: 120%;
    padding: 0.6% 2%;
    border: none;
    border-radius: 6px;
    margin-left: 6%;
}

.container-profile-bar {
    margin-left: 2%;
    width: 15%;
    height: 60%;
    border-radius: 33px;
    display: flex;
    align-items: center;
    background-color: #131b26;
}

.coin-image {
    margin-left: 8%;
    background-image: url("./image-src/background-coin.png");
    background-repeat: no-repeat;
    background-position: center -10px;

}

.column-coin {
    margin-left: 4%;
    font-size: 110%;
    color: #ffffff;
    font-weight: bold;
    font-family: "Avenir Next Cyr";
}

.column-money {
    margin-left: 4%;
    font-size: 110%;
    color: #ffffff;
    font-weight: bold;
    font-family: "Avenir Next Cyr";
}

.profile-icon {
    margin-left: 3%;
    border-width: 1px;
    border-color: rgb(75, 94, 127);
    border-style: solid;
    border-radius: 50%;
    background-color: rgb(158, 69, 227);

    /* Окно самого профиля */
    width: 50px;
    height: 50px;
    background-image: url('./image-src/test-profile.png');
    background-position: center;
    background-size: cover;
}

</style>