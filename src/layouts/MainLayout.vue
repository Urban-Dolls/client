<template>
  <div class="page-container">
    <!-- sidebar menu area start -->
    <div class="sidebar-menu">
        <div class="sidebar-header">
            <div class="logo">
                <a href="index.html">
                    <!-- <img src="assets/images/icon/logo.png" alt="InvenDolls"> -->
                    IvenDolls
                </a>
            </div>
        </div>
        <div class="main-menu">
            <div class="menu-inner">
                <nav>
                    <ul class="metismenu" id="menu">
                        <li class="active">
                            <a href="javascript:void(0)" aria-expanded="true">
                                <i class="ti-dashboard"></i>
                                <span>Inicio</span>
                            </a>
                            <ul class="collapse">
                                <li class="active">
                                    <a href="/inicio.html">
                                        Floresta
                                    </a>
                                </li>
                                <li>
                                    <a href="/inicio.html">
                                        Santa Lucía
                                    </a>
                                </li>
                            </ul>
                        </li>
                        <li>
                            <a href="/ventas.html"><i
                                    class="ti-receipt"></i><span>Ventas
                                </span></a>
                        </li>
                        <li>
                            <a href="/productos.html"><i
                                    class="ti-package"></i><span>Productos</span></a>
                        </li>
                        <li>
                            <a href="/clientes.html"><i class="ti-user"></i><span>Clientes</span></a>
                        </li>
                        <li>
                            <a href="javascript:void(0)" aria-expanded="true"><i
                                    class="ti-pie-chart"></i><span>Reportes</span></a>
                            <ul class="collapse">
                                <li><a href="/reportes-ventas.html">Por Ventas</a></li>
                                <li><a href="/reportes-inventario.html">Por Inventario</a></li>
                            </ul>
                        </li>
                        <li>
                            <a href="javascript:void(0)" aria-expanded="true"><i class="ti-settings"></i>
                                <span>Configuración</span></a>
                            <ul class="collapse">
                                <li><a href="/usuarios.html">Usuarios</a></li>
                                <li><a href="/roles.html">Roles</a></li>
                                <li><a href="/almacenes.html">Almacenes</a></li>
                            </ul>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </div>
    <!-- sidebar menu area end -->
    <!-- main content area start -->
    <div class="main-content">
        <!-- header area start -->
        <div class="header-area">
            <div class="row align-items-center">
                <!-- nav and search button -->
                <div class="col-md-6 col-sm-8 clearfix">
                    <div class="nav-btn pull-left">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <div class="search-box pull-left">
                        <form action="#">
                            <input type="text" name="search" placeholder="Buscar..." required>
                            <i class="ti-search"></i>
                        </form>
                    </div>
                </div>
                <!-- profile info & task notification -->
                <div class="col-md-6 col-sm-4 clearfix">
                    <ul class="notification-area pull-right">
                        <li class="settings-btn">
                            <i class="ti-settings"></i>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <!-- header area end -->
        <!-- page title area start -->
        <div class="page-title-area">
            <div class="row align-items-center">
                <div class="col-sm-6">
                    <div class="breadcrumbs-area clearfix">
                        <h4 class="page-title pull-left">{PAGE TITLE}</h4>
                    </div>
                </div>
                <div class="col-sm-6 clearfix">
                    <div class="user-profile pull-right">
                        <img class="avatar user-thumb" src="static/images/avatar.png" alt="avatar">
                        <h4 class="user-name dropdown-toggle" data-toggle="dropdown">Sofía Pérez <i
                                class="fa fa-angle-down"></i></h4>
                        <div class="dropdown-menu">
                            <a class="dropdown-item" href="#">Cerrar sesión</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- page title area end -->
        <div class="main-content-inner">
          <router-view />
        </div>
    </div>
    <!-- main content area end -->
    <!-- footer area start-->
    <footer>
      <div class="footer-area">
        <p>
          Urban Dolls © Copyright 2019. Todos los derechos reservados.
        </p>
      </div>
    </footer>
    <!-- footer area end-->
  </div>
</template>

<script>
export default {
  name: 'MainLayout'
}
</script>
