<template>
    <div class="dark-mode">
<div class="wrapper">

  <!-- Preloader -->
  <!-- <div class="preloader flex-column justify-content-center align-items-center">
    <img class="animation__wobble" src="dist/img/AdminLTELogo.png" alt="AdminLTELogo" height="60" width="60">
  </div>  -->

  <!-- Navbar -->
    <NavBar />
  <!-- /.navbar -->

  <!-- Main Sidebar Container -->
    <SideBar />

  <!-- Content Wrapper. Contains page content -->
  <div class="content-wrapper">
    <!-- Content Header (Page header) -->
    <div class="content-header">
      <div class="container-fluid">
        <div class="row mb-2">
          <div class="col-sm-6">
              <slot name="header"></slot>
          </div><!-- /.col -->
        </div><!-- /.row -->
      </div><!-- /.container-fluid -->
    </div>
    <!-- /.content-header -->

    <!-- Main content -->
        <slot></slot>
    <!-- /.content -->
  </div>
  <!-- /.content-wrapper -->

  <!-- Main Footer -->
    <Footer />
</div>
</div>
</template>

<script>
    import Footer from '@/Components/Footer'
    import NavBar from '@/Components/NavBar'
    import SideBar from '@/Components/SideBar'
    export default {
        components: {
          Footer,
          NavBar,
          SideBar,
        }
    }
</script>