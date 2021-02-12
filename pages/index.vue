<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light navbar-95 ">
        <a class="navbar-brand" href="#"><img src="logo_phil.png" class="icon-32"> Philsbude</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown"
            aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                </li>

                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button"
                        data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Buchung
                    </a>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
                        <a class="dropdown-item" href="#">Nur n Joke, bin unbezahlbar</a>

                    </div>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#" @click="maMan">Mein Tipp an dich!</a>
                </li>
            </ul>
        </div>
    </nav>
    <div class="header mb-5 cool">
       <div class="container h-100">
            <div class="d-flex justify-content-center h-100 align-items-center">
                <div class="card" style="width: 60vh;">
                    <div class="card-header icon">
                        <h4 class="my-0 font-weight-normal ">
                            <img src="phil.png" class="icon-32"> Über mich
                        </h4>
                    </div>
                    <div class="card-body">
                        <ul class="list-unstyled mt-3 mb-4">
                            <li>Hi, ich bin Phil</li>
                            <li>Twitch streamer aus Würzburg</li>
                        </ul>
                        <div class="btn-group btn-block" role="group" aria-label="Basic example">
                            <a class="btn btn-secondary" href="https://www.twitch.tv/philsbude">
                                 Twitch
                            </a>
                            <a class="btn btn-secondary"
                                href="https://www.youtube.com/channel/UCXaziuVsJOs-527gi3HkXsg">
                                Youtube
                            </a>
                            <a class="btn btn-secondary" href="https://www.instagram.com/phils_bude/">
                                Instagram
                            </a>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="myModal" class="modal" @click="maMan">

  <!-- Modal content -->
  <div class="modal-content">
    <img src="ThatMan2.gif">
  </div>

</div>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    methods:{
        maMan(){
            document.getElementById("myModal")?.classList.toggle("open")
        }
    }
})
</script>

<style>
 /* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.4); /* Black w/ opacity */
}

.modal.open {
    display: block;
}

/* Modal Content/Box */
.modal-content {
  background-color: #fefefe;
  margin: 15% auto; /* 15% from the top and centered */
  padding: 20px;
  border: 1px solid #888;
  width: 80%; /* Could be more or less, depending on screen size */
}

/* The Close Button */
.close {
  color: #aaa;
  float: right;
  font-size: 28px;
  font-weight: bold;
}

.close:hover,
.close:focus {
  color: black;
  text-decoration: none;
  cursor: pointer;
} 
</style>