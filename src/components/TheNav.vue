<template>
  <div>
    <nav class="navbar">
      <div class="brand-title">
          <img src="../assets/svgs/NavLogoDark.svg" alt="Scales Emporium Logo">
      </div>
      <a href="#" class="toggle-button" @click="ShowMenu">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </a>
      <div class="navbar-links">
        <ul>
          <li><a href="">Products</a></li>
          <li><a href="">About</a></li>
          <li><a href="">Cart</a></li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script setup>

// Hamburger On click 
    function ShowMenu () {
    const navbarLinks = document.getElementsByClassName('navbar-links')[0];
    navbarLinks.classList.toggle('active')
  }
</script>

<style >
:root {
  --primary-color:  #D5E5E4; /* green 100*/
  --secondary-color: #050D0C; /* green 900*/
  --tertiary-color:  #235F5A; /* green 600*/
  --quaternary-color: #173F3C; /* green 700*/
}

  /* Navbar styles  */
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: var(--tertiary-color);
    color: var(--primary-color);
    text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.25);
  }

  .brand-title {
    display: block;
    padding-top: 0.5rem;
    object-fit: contain;
    width: 90%;
    min-width: 20%;
    margin: 5px 0 5px 20px;

  }

  .brand-title img {
    object-fit: contain;
    width: 100%;
    max-width: 18%;
  }

  .navbar-links {
    margin-right: 2%;
  }
  .navbar-links ul{
    margin: 0;
    padding: 0;
    display: flex;
  }

  .navbar-links li {
    list-style: none;
  }

  .navbar-links li a {
    text-decoration: none;
    color: white;
    padding: 1rem;
    display: block;
    font-size: 1.5rem;
  }

  /* Hamburger styles  */
  .toggle-button {
    position: absolute;
    top: 0.75rem;
    right: 1rem;
    display: none;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 21px;
    
  }
  .toggle-button .bar {
    height: 3px;
    width:100%;
    background-color: white;
    border-radius: 10px;
  }
  @media (max-width: 800px) {
    .toggle-button {
      display: flex;
    }
    .navbar-links{
      display: none;
      width: 100%
    }
    .navbar {
      flex-direction: column;
      align-items: flex-start;
    }
    .navbar-links ul{
      width: 100%;
      flex-direction: column;
    }
    .navbar-links ul li {
      text-align: center;
    }
    .navbar-links li a {
      padding: 0.5rem 1rem;
    }
    .navbar-links.active {
      display: flex;
    }
  }

  /* Hover  */
  .navbar-links li a:hover{
    color: var(--secondary-color);
  }

</style>