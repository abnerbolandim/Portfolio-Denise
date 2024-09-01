<template>
    <div id="app">
      <!-- Mapa do Leaflet -->
      <div id="map" class="map-container"></div>
  
      <footer class="footer">
        <div class="footer-container">
          <div class="footer-section logo-section">
            <img src="../assets/IconDeniseBlack.png" alt="Logo Denise" class="logo" />
            <div class="social-icons">
              <a href="#" class="icon facebook-icon"><i class="fab fa-facebook"></i></a>
              <a href="#" class="icon instagram-icon"><i class="fab fa-instagram"></i></a>
            </div>
            <p>Desde 2023 <br>©  DENISE Bolos & Salgados</p>
          </div>
          <div class="footer-section links-section">
            <h4>HOME PAGE</h4>
            <ul>
              <li><a href="#">INÍCIO</a></li>
              <li><a href="#">PRODUTOS</a></li>
              <li><a href="#">SOBRE</a></li>
              <li><a href="#">LOCALIZAÇÃO</a></li>
              <li><a href="#">CONTATO</a></li>
            </ul>
          </div>
          <div class="footer-section contact-section">
            <h4>CONTATO</h4>
            <p>Delivery: <br>+351 987654321</p>
            <p>
              Informações:
              <a href="..."><br>marketing@denise.com.br</a>
            </p>
          </div>
        </div>
      </footer>
    </div>
  </template>
  
  <script>
  import L from 'leaflet';
  
  export default {
    name: 'App',
    mounted() {
      
      const map = L.map('map').setView([38.736946, -9.142685], 13); 
  
      
      L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '© OpenStreetMap contributors'
      }).addTo(map);
  
      
      L.marker([38.736946, -9.142685]).addTo(map)
        .bindPopup('Estamos aqui em Portugal!')
        .openPopup();
    }
  };
  </script>
  
  <style scoped>
  #app {
    font-family: Arial, sans-serif;
    justify-content: center;
    background-color: #e8dddd;
  }
  
  .map-container {
  width: 70%;
  height: 400px;
  padding-bottom: 20px;
  position: relative;
  background-color: #f0f0f0; 
}


  .footer {
    background-color: #e8dddd;
    padding: 20px;
    color: black;
    font-family: 'Arial', sans-serif;
    z-index: 1; 
    position: relative; 
  }
  
  .footer-container {
    display: flex;
    justify-content: space-between;
  }
  
  .footer-section {
    flex: 1;
    margin: 10px;
  }
  
  .logo-section .logo {
    width: 100px;
  }
  
  .social-icons {
    display: flex;
    gap: 10px;
    margin: 10px 0;
  }
  
  .social-icons .icon {
    font-size: 24px;
    color: #810947;
  }
  
  .facebook-icon i {
    background-color: #810947;
    border-radius: 50%;
    padding: 10px;
    color: white;
  }
  
  .instagram-icon i {
    background-color: #810947;
    border-radius: 50%;
    padding: 11px;
    color: white;
  }
  
  .links-section ul {
    list-style: none;
    padding: 0;
  }
  
  .links-section ul li {
    margin-bottom: 8px;
  }
  
  .links-section ul li a {
    color: #810947;
    text-decoration: none;
  }
  
  .contact-section p {
    margin: 8px 0;
  }
  
  .contact-section a {
    color: black;
    text-decoration: none;
  }
  
  @media (max-width: 655px) {
    .links-section {
      display: none;
    }
  }
  </style>
  