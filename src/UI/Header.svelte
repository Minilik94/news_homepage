<script>
  let headerNav;
  let hum;
  let times;
  let dav;
  let active = false;

  function toggleNav() {
    headerNav = document.querySelector(".header");
    hum = document.querySelector(".hum");
    times = document.querySelector(".times");
    dav = document.getElementById("dav");

    if (!active) {
      headerNav.classList.add("active");
      hum.classList.remove("active");
      dav.classList.add("active");
      times.style.display = "block";
      active = true;
    } else {
      headerNav.classList.remove("active");
      hum.classList.add("active");
      dav.classList.remove("active");
      times.style.display = "none";
      active = false;
    }
  }
</script>

<header class="header">
  <!-- Add the logo -->
  <a href="#" class="logo"><img src="../images/logo.svg" alt="logo" /></a>

  <!-- Add the navigation -->
  <div id="dav" class="">
    <nav>
      <a href="#">Home</a>
      <a href="#">New</a>
      <a href="#">Popular</a>
      <a href="#">Trending</a>
      <a href="#">Catagories</a>
    </nav>
  </div>

  <div class="mobile-nav">
    <a href="#" class="hum active" on:click={toggleNav}
      ><img src="../images/icon-menu.svg" alt="" /></a
    >
    <a href="#" class="times" on:click={toggleNav}
      ><img src="../images/icon-menu-close.svg" alt="" /></a
    >
  </div>
</header>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  .mobile-nav {
    display: none;
  }
  /* Style the header */
  /* Style the header for screens larger than 850px */
  .header {
    display: flex;
    align-items: center;
    width: 100%;
    height: 50px;
    padding: 0 3rem;
    justify-content: space-between;
  }

  /* Style the logo for screens larger than 850px */
  .header .logo {
    margin-right: 50px;
    font-size: 20px;
    text-decoration: none;
    transition: all 0.3s ease;
  }

  /* Style the navigation elements for screens larger than 850px */
  .header nav {
    display: flex;
  }
  .header nav a {
    margin: 0 10px;
    text-decoration: none;
    font-size: 16px;
    transition: all 0.3s ease;
    color: #000;
  }

  /* Style the header, logo, and navigation elements for screens smaller than 850px */
  @media (max-width: 850px) {
    .header {
      flex-wrap: nowrap;
      justify-content: space-between;
      padding-left: 1rem;
      padding-right: 1rem;
    }
    .header .logo {
      margin-right: 0;
      margin-bottom: 10px;
      margin-top: 10px;
      margin-left: 0;
      padding-left: 0;
    }
    .header nav {
      flex-wrap: nowrap;
    }
    .header nav a {
      margin: 0 5px;
      padding: 0 5px;
      font-size: 14px;
    }
  }
  @media (max-width: 698px) {
    .mobile-nav {
      display: flex;
      position: relative;
      height: 40px;
      width: 50px;
    }
    .mobile-nav .hum,
    .mobile-nav .times {
      position: absolute;
      top: 10%;
      right: 0;
      z-index: 100;
    }
    .mobile-nav .times {
      display: none;
    }
    .mobile-nav .hum {
      display: none;
    }
    .mobile-nav .hum {
      padding: 0.2rem 00.2rem 0rem 0;
    }
    .mobile-nav .hum.active {
      display: block;
    }

    .header nav {
      display: none;
      transition: all 0.7s ease;
    }

    .header .active nav {
      position: absolute;
      top: 0%;
      right: 0%;
      display: flex;
      flex-direction: column;
      height: 305%;
      z-index: 1;
      background: #fff;
      padding: 26% 15rem 0 1rem;
      transition: all 0.6s ease;
    }
    .header nav a {
      padding: 0.5rem;
      font-family: "Inter", sans-serif;
      font-size: 1.5rem;
    }
  }
</style>
