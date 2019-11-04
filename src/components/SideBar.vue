<template>
  <div class='sidebar-menu' :style="{ left: isVisible ? 0 : '-90%' }">
    <div class='sidebar-header'>
      <div class='logo'>
        <a href='/'>
          <!-- <img src='assets/images/icon/logo.png' alt='InvenDolls'> -->
          IvenDolls
        </a>
      </div>
    </div>
    <div class='main-menu'>
      <div class='menu-inner'>
        <nav>
          <ul class='metismenu' id='menu'>
            <li class='active'>
              <a href='javascript:void(0)' aria-expanded='true'>
                <i class='ti-dashboard'></i>
                <span>Inicio</span>
              </a>
              <ul class='collapse'>
                <li class='active'>
                  <a href='/inicio.html'>Floresta</a>
                </li>
                <li>
                  <a href='/inicio.html'>Santa Lucía</a>
                </li>
              </ul>
            </li>
            <li>
              <a href='/ventas.html'>
                <i class='ti-receipt'></i>
                <span>Ventas</span>
              </a>
            </li>
            <li>
              <a href='/productos.html'>
                <i class='ti-package'></i>
                <span>Productos</span>
              </a>
            </li>
            <li>
              <a href='/clientes.html'>
                <i class='ti-user'></i>
                <span>Clientes</span>
              </a>
            </li>
            <li>
              <a href='javascript:void(0)' aria-expanded='true'>
                <i class='ti-pie-chart'></i>
                <span>Reportes</span>
              </a>
              <ul class='collapse'>
                <li>
                  <a href='/reportes-ventas.html'>Por Ventas</a>
                </li>
                <li>
                  <a href='/reportes-inventario.html'>Por Inventario</a>
                </li>
              </ul>
            </li>
            <li>
              <a href='javascript:void(0)' aria-expanded='true'>
                <i class='ti-settings'></i>
                <span>Configuración</span>
              </a>
              <ul class='collapse'>
                <li>
                  <a href='/usuarios.html'>Usuarios</a>
                </li>
                <li>
                  <a href='/roles.html'>Roles</a>
                </li>
                <li>
                  <a href='/almacenes.html'>Almacenes</a>
                </li>
              </ul>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SideBar',
  props: {
    title: {
      type: Object,
      // required: true,
      default: () => ({
        title: '',
        url: null,
        logo: null
      })
    },
    items: {
      type: Array,
      // required: true,
      default: () => []
    },
    isVisible: {
      type: Boolean,
      required: true,
      default: false
    }
  }
}
</script>
