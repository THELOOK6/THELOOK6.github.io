<template>
  <div class="ComingSoonMainContainer">
    <div class="coming-soon">
      <div class="background"></div>
      <div class="overlay"></div>
      <div class="content">
        <h2>En Developpement</h2>
        <h4>gabriel.look.dev@gmail.com</h4>
      </div>
    </div>
  </div>
</template>

<style>
@font-face {
  font-family: "Helvetica 87 Heavy Condensed Oblique";
  src: url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.eot");
  src: url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.eot?#iefix")format("embedded-opentype"),
    url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.woff2")format("woff2"),
    url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.woff")format("woff"),
    url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.ttf")format("truetype"),
    url("https://db.onlinewebfonts.com/t/3fe222a6b4ff5a85138b24f64f19e59c.svg#Helvetica 87 Heavy Condensed Oblique")format("svg");
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}


@media (min-width: 1024px) {

  .ComingSoonMainContainer{
    padding: 0;
    margin: 0;
    width: 100vw;
    height: 100vh;
  
  }

  .coming-soon {
    position: relative;
    height: 100%;
    display: block;
    justify-content: center;
    align-items: center;
  }

  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url('../assets/coding_background.jpg') no-repeat center center/cover;
    filter: blur(10px);
    z-index: -2;
  }

  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
  }



  .content {
    position: relative;
    height: 100%;  
    text-align: center;
    justify-content: center;
    align-content: center;
    color: white;
    opacity: 0;
    animation: fadeIn 8s forwards;
  }


  h2 {
    font-family: "Helvetica 87 Heavy Condensed Oblique";
    font-size: 7rem;
  }
  
  h4 {
    font-family: "Helvetica 87 Heavy Condensed Oblique";
    font-size: 2rem;
  }

}
</style>
