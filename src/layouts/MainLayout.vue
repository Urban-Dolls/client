<template>
  <div class="page-container">
    <SideBar :isVisible="false" />
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
import SideBar from '../components/SideBar'

export default {
  name: 'MainLayout',
  components: {
    SideBar
  }
}
</script>
