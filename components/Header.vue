<template>
  <!--Main Navigation-->
  <header>
    <!-- Sidebar -->
    <nav id="sidenav-1" class="sidenav" data-mdb-hidden="true">
      <ul class="sidenav-menu">
        <li class="sidenav-item">
          <a class="navbar-brand" href="#">
            Browse the Community
          </a>
        </li>
        <li class="sidenav-item">
          <a class="sidenav-link" href="/">
            <i class="far fa-smile fa-fw me-3"></i><span>Home</span></a>
        </li>
        <li class="sidenav-item">
          <a class="sidenav-link" href="/members">
            <i class="far fa-smile fa-fw me-3"></i><span>Browse Members</span></a>
        </li>
        <li class="sidenav-item">
          <a class="sidenav-link" href="/channel/">
            <i class="far fa-smile fa-fw me-3"></i><span>Channels</span></a>
        </li>
        <li class="sidenav-item">
          <a class="sidenav-link" href="/game/">
            <i class="far fa-smile fa-fw me-3"></i><span>Games</span></a>
        </li>
        <li class="sidenav-item">
          <a class="sidenav-link" href="/journal/">
            <i class="far fa-smile fa-fw me-3"></i><span>Journals</span></a>
        </li>
      </ul>
    </nav>
    <!-- Sidebar -->

    <!-- Navbar -->
    <nav id="main-navbar" class="navbar navbar-expand-lg navbar-light bg-white fixed-top">
      <!-- Container wrapper -->
      <div class="container-fluid">
        <!-- Toggle button -->
        <button data-mdb-toggle="sidenav" data-mdb-target="#sidenav-1" class="btn btn-primary"
          aria-controls="#sidenav-1" aria-haspopup="true">
          <i class="fas fa-bars"> Menu</i>
        </button>

        <!-- Brand -->
        <a class="navbar-brand" href="#">
         <img src="../static/logo.png" alt="HERE2MINGLE"> HERE2MINGLE
        </a>
        <!-- Search form -->
        <div class="collapse navbar-collapse justify-content-center" id="navbarCenteredExample">
          <form class="d-none d-md-flex input-group w-auto my-auto">
            <input autocomplete="off" type="search" class="form-control rounded"
              placeholder='Search the Community' style="width: 525px;">
            <span class="input-group-text rounded border-1"><i class="fas fa-search"></i></span>
          </form>
        </div>
        <!-- Right links -->
        <ul class="navbar-nav ms-auto d-flex flex-row">
          <li class="nav-item">
            <a class="nav-link me-3 me-lg-0" role="button" aria-expanded="false" href="/social/newsfeed"><i class="fas fa-comment-alt"></i></a>
          </li>
          <li class="nav-item">
            <a class="nav-link me-3 me-lg-0" role="button" aria-expanded="false" href="/social/groups"><i class="fas fa-users"></i></a>
          </li>
          <!-- Notification dropdown -->
          <li class="nav-item dropdown">
            <a class="nav-link me-3 me-lg-0 dropdown-toggle hidden-arrow" href="#" id="navbarDropdownMenuLink"
              role="button" data-mdb-toggle="dropdown" aria-expanded="false">
              <i class="fas fa-bell"></i>
              <span class="badge rounded-pill badge-notification bg-danger">1</span>
            </a>
            <ul class="dropdown-menu dropdown-menu-end" aria-labelledby="navbarDropdownMenuLink">
              <li>
                <a class="dropdown-item" href="#">Some news</a>
              </li>
              <li>
                <a class="dropdown-item" href="#">Another news</a>
              </li>
              <li>
                <a class="dropdown-item" href="#">Something else here</a>
              </li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link me-3 me-lg-0 dropdown-toggle hidden-arrow" href="#" id="navbarDropdownMenuLink"
              role="button" data-mdb-toggle="dropdown" aria-expanded="false">
              <i class="fas fa-user-circle"></i>
            </a>
            <ul class="dropdown-menu dropdown-menu-end" aria-labelledby="navbarDropdownMenuLink">
              <li>
                <a class="dropdown-item" href="#">My profile</a>
              </li>
              <li>
                <a class="dropdown-item" href="#">Settings</a>
              </li>
              <li>
                <a class="dropdown-item" href="#">Logout</a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
      <!-- Container wrapper -->
    </nav>
    <!-- Navbar -->
  </header>
</template>

<style>

</style>
