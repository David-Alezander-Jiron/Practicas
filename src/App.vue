<template>
  <div id="app">
    <SidebarMenu />
    <div class="main-content">
      <div>
        <div class="sidebar">
          <div class="logo">
            <img src="@/assets/logopra.png" alt="Eventix Logo" />
          </div>
          <nav class="navigation">
            <ul>
              <li>
                <a href="#"><img src="@/assets/iconodash.png" class="menu-icon" alt="Dashboard Icon" /> Dashboard</a>
              </li>
              <li>
                <a href="#">Email</a>
              </li>
              <li>
                <a href="#">Widgets <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">UI Elements <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Registros</a>
              </li>
              <li>
                <a href="#">Eventos <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Administrador</a>
              </li>
              <li>
                <a href="#">Gestion <span class="new-badge">NEW</span></a>
              </li>
              <li class="submenu">
                <a href="#" @click="toggleSubMenu">Gestion Entradas <i :class="{'fa fa-chevron-down': !submenuOpen, 'fa fa-chevron-up': submenuOpen}"></i></a>
                <ul v-if="submenuOpen">
                  <li><a href="#">Listado de entradas</a></li>
                  <li><a href="#">Detalle de entrada</a></li>
                </ul>
              </li>
              <li>
                <a href="#">Front End <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Email Template</a>
              </li>
              <li>
                <a href="#">Chart</a>
              </li>
              <li>
                <a href="#">Calendar</a>
              </li>
              <li>
                <a href="#">Map</a>
              </li>
              <li>
                <a href="#">Gallery</a>
              </li>
              <li>
                <a href="#">Page Options <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Extra <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Login & Register</a>
              </li>
              <li>
                <a href="#">Version <span class="new-badge">NEW</span></a>
              </li>
              <li>
                <a href="#">Helper</a>
              </li>
              <li>
                <a href="#">Menu Level</a>
              </li>
            </ul>
          </nav>
        </div>

        <div class="topbar">
          <div class="search-bar">
            <input type="text" placeholder="Enter keyword" />
            <img src="@/assets/campana.png" alt="Icono de campana" />
          </div>
          <div class="topbar-icons">
            <img src="@/assets/persona.png" alt="Avatar" class="avatar" />
            <span>Administrador</span>
            <i class="fa fa-user"></i>
          </div>
        </div>

        <div class="menu-below-topbar">
          <ul>
            <li><a href="#">Dashboard/</a></li>
            <li><a href="#">Usuarios/</a></li>
            <li><a href="#">Home</a></li>
          </ul>
        </div>

        <div class="stat-cards">
          <div class="stat-card">
            <div class="stat-icon">
              <img src="@/assets/stacts1.png" alt="Icon 1" />
            </div>
            <div class="stat-info">
              <h3>Usuarios Registrados</h3>
              <p>7,842,900</p>
              <a href="#">Todos los detalles aquí</a>
            </div>
          </div>
          <div class="stat-card">
            <div class="stat-icon">
              <img src="@/assets/stacts2.png" alt="Icon 2" />
            </div>
            <div class="stat-info">
              <h3>Ventas de Tickets</h3>
              <p>180,200</p>
              <a href="#">Todos los detalles aquí</a>
            </div>
          </div>
          <div class="stat-card">
            <div class="stat-icon">
              <img src="@/assets/stacts3.png" alt="Icon 3" />
            </div>
            <div class="stat-info">
              <h3>Eventos Próximos</h3>
              <p>38,900</p>
              <a href="#">Todos los detalles aquí</a>
            </div>
          </div>
          <div class="stat-card">
            <div class="stat-icon">
              <img src="@/assets/stacts4.png" alt="Icon 4" />
            </div>
            <div class="stat-info">
              <h3>Nuevos Comentarios</h3>
              <p>3,988</p>
              <a href="#">Todos los detalles aquí</a>
            </div>
          </div>
        </div>
      </div>

      <div class="notification-cards">
          <div class="card notification-card">
            <h3>Notificaciones</h3>
            <p>Nuevas notificaciones de las ventas de tickets del evento Proximo a destacar</p>
            <a href="#">Ver detalles</a>
            <span class="notification-dot"></span>
          </div>
          <div class="card event-card">
            <div class="ticket">
              <div class="ticket-details">
                <h3>NOMBRE DEL EVENTO</h3>
                <p>@ DEL EVENTO</p>
                <p>10/12/2023 | 10:00 PM</p>
                <p>ACCESO 21:00 PM</p>
                <p>PALCO FICO'S</p>
                <p>¡Un evento inigualable!</p>
              </div>
              <div class="ticket-price">
                <p>$18</p>
              </div>
            </div>
          </div>
        </div>
      </div>
     
      <div class="extra-cards">
          <div class="card highlight-events-card">
            <h3>Próximos eventos a destacar</h3>
            <div class="highlight-event">
              <h4>Concierto de rock</h4>
              <p>Fecha: 20 de Julio, 2024</p>
              <p>Ubicación: Estadio Nacional</p>
              <p>Descripción: Un increíble concierto con las mejores bandas de rock del momento.</p>
            </div>
            <div class="highlight-event">
              <h4>Feria de Tecnología</h4>
              <p>Fecha: 15 de Agosto, 2024</p>
              <p>Ubicación: Centro de Convenciones</p>
              <p>Descripción: La feria más grande de tecnología con expositores de todo el mundo.</p>
            </div>
            <div class="highlight-event">
              <h4>Festival de Cine</h4>
              <p>Fecha: 5 de Septiembre, 2024</p>
              <p>Ubicación: Teatro Principal</p>
              <p>Descripción: Disfruta de las mejores películas y cortometrajes del año.</p>
            </div>
            <div class="highlight-event">
              <h4>Evento de Jazz en el Parque</h4>
              <p>Fecha: 10 de Octubre, 2024</p>
              <p>Ubicación: Parque Central</p>
              <p>Descripción: Únete a nosotros para una velada inolvidable de jazz bajo las estrellas.</p>
            </div>
          </div>
          <div class="card map-card">
            <h3>Vista del mapa de más ventas de tickets de eventos</h3>
            <div class="map-details">
              <p><strong>Mapa tiempo real</strong></p>
              <p>08 de julio de 2024</p>
              <img src="@/assets/mapa.png" alt="Mapa" />
            </div>
          </div>
        </div>
      </div>

      <MyComponent />
</template>

<script>
import SidebarMenu from './components/SidebarMenu.vue';
import MyComponent from './components/MyComponent.vue';

export default {
  name: 'App',
  components: {
    SidebarMenu,
    MyComponent
  }
}
</script>

<style scoped>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  overflow-x: hidden; /* Evita el desplazamiento horizontal */
}

.sidebar {
  width: 250px;
  background-color: #d9d9d9;
  height: 100vh;
  position: fixed;
  top: 0;
  overflow-y: auto;
  padding-top: 60px; /* Ajustar para que el contenido comience más arriba */
}

.logo {
  text-align: center;
  padding: 20px 0;
}

.logo img {
  width: 150px;
  border-radius: 15px;
}

.navigation {
  padding: 0;
}

.navigation ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.navigation ul li {
  padding: 10px 20px;
}

.navigation ul li a {
  text-decoration: none;
  color: #8c9094;
  display: flex;
  align-items: center;
}

.navigation ul li a:hover {
  background-color: #20252a;
}

.new-badge {
  background-color: #00acac;
  color: #fff;
  font-size: 12px;
  padding: 2px 5px;
  border-radius: 3px;
  margin-left: auto; /* Añade esto para empujar el badge a la derecha */
}

.submenu ul {
  padding-left: 20px;
}

.submenu ul li a {
  font-size: 14px;
}

.fa {
  margin-left: 10px;
}

.menu-icon {
  width: 20px;
  margin-right: 10px;
}

.topbar {
  margin-left: 250px; /* Ajustar el margen izquierdo para que no se superponga con la barra lateral */
  background-color: #f8f9fa;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  border-bottom: 1px solid #dee2e6;
  position: fixed;
  top: 0;
  width: calc(100% - 250px); /* Ajustar al ancho menos el ancho de la barra lateral */
  z-index: 1000;
}

.search-bar {
  display: flex;
  align-items: center;
}

.search-bar input {
  padding: 5px;
  border: 1px solid #ced4da;
  border-radius: 15px;
  width: 310px; /* Ajusta el ancho según necesites */
  margin-left: 300px;
}

.search-bar img {
  width: 50px; /* Ajusta el tamaño de la imagen de la campana */
  margin-left: 10px; /* Espacio entre el input y la imagen de la campana */
  cursor: pointer;
}

.topbar-icons {
  display: flex;
  align-items: center;
}

.topbar-icons img.avatar {
  width: 50px; /* Ajusta el tamaño del avatar */
  height: 40px;
  border-radius: 50%; /* Para redondear la imagen */
  margin-right: 10px; /* Espacio entre la imagen y el texto */
}

.topbar-icons span {
  margin-right: 150px; /* Ajusta el espacio entre "Administrador" y el icono de usuario */
}

.topbar-icons i {
  margin: 0 10px; /* Espacio entre los iconos en la barra superior */
  cursor: pointer;
}

.menu-below-topbar {
  margin-top: 60px; /* Ajusta este valor para mover el menú más arriba o más abajo */
  margin-left: 250px; /* Ajusta el margen izquierdo para alinear con la barra lateral */
  padding: 10px 20px;
  background-color: #f8f9fa;
  border-bottom: 1px solid #dee2e6;
  display: flex;
  align-items: center;
}

.menu-below-topbar ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 20px;
}

.menu-below-topbar ul li {
  padding: 10px 0;
}

.menu-below-topbar ul li a {
  text-decoration: none;
  color: #000;
}

.menu-below-topbar ul li a:hover {
  text-decoration: underline;
}

.stat-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  display: flex;
  align-items: center;
  padding: 20px;
  min-width: 190px; /* Establece un ancho mínimo */
  max-width: 100%; /* Permite que las cartas crezcan según el contenido */
  margin: 10px; /* Espacio entre las cartas */
  position: relative;
  overflow: hidden;
}

.stat-icon {
  position: absolute;
  top: 10px;
  right: 10px;
}

.stat-icon img {
  width: 220px; /* Ajusta el tamaño del ícono según sea necesario */
  height: 100px;
}

.stat-info {
  z-index: 1;
}

.stat-info h3 {
  margin: 0;
  font-size: 18px;
  color: #fff;
}

.stat-info p {
  margin: 5px 0;
  font-size: 24px;
  font-weight: bold;
  color: #fff;
}

.stat-info a {
  color: #fff;
  text-decoration: none;
}

.stat-info a:hover {
  text-decoration: underline;
}

.stat-cards {
  display: flex;
  padding: 10px;
  margin-left: 250px; /* Ajusta el margen para que coincida con la barra lateral */
}

.notification-cards {
  display: flex;
  gap: 20px;
  margin-top: 20px;
  margin-left: 250px; /* Ajusta el margen para que coincida con la barra lateral */
}

.card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 20px;
  width: 100%;
  position: relative;
}

.notification-card h3 {
  margin: 0 0 10px;
  font-size: 18px;
}

.notification-card p {
  margin: 0 0 10px;
  color: #555;
}

.notification-card a {
  color: #007bff;
  text-decoration: none;
  font-weight: bold;
}

.notification-dot {
  width: 10px;
  height: 10px;
  background-color: red;
  border-radius: 50%;
  position: absolute;
  top: 10px;
  right: 10px;
}

.event-card .ticket {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.ticket-details h3 {
  margin: 0 0 5px;
  font-size: 18px;
}

.ticket-details p {
  margin: 0 0 5px;
  color: #555;
}

.ticket-price p {
  font-size: 24px;
  font-weight: bold;
  color: #000;
}


/*tarjetas terceras */
.extra-cards {
  display: flex;
  gap: 20px;
  margin-top: 20px;
  margin-left: 250px; /* Ajusta el margen para que coincida con la barra lateral */
}

.card.highlight-events-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 20px;
  width: 100%;
}

.card.map-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 20px;
  width: 100%;
}

.highlight-events-card h3,
.map-card h3 {
  margin-bottom: 20px;
  font-size: 24px;
}

.highlight-event {
  background-color: #D8D2BF;
  border-radius: 8px;
  padding: 10px;
  margin-bottom: 10px;
}

.highlight-event h4 {
  margin: 0 0 5px;
  font-size: 18px;
}

.highlight-event p {
  margin: 0 0 5px;
  color: #555;
}

.map-details p {
  margin: 0 0 10px;
  font-size: 16px;
}

.map-details img {
  width: 100%;
  border-radius: 8px;
}


</style>
