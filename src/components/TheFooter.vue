<template>
  <div class="footer-container">
    <div class="footer-items">
      <h2>About Us</h2>
      <ul>
        <li> <a href="#" target="_blank"> Giving Back</a>  </li>
        <li> <a href="#" target="_blank"> Careers </a>  </li>
        <li> <a href="#" target="_blank"> Customer Care Policy </a>  </li>
      </ul>
    </div>
    <div class="footer-items">
      <h2>Our Stores</h2>
      <ul>
        <li> <a href="#" target="_blank"> Store Locator </a>  </li>
        <li> <a href="#" target="_blank"> Services </a>  </li>
      </ul>
    </div>
    <div class="footer-items">
      <h2>Learn More</h2>
      <ul>
        <li> <a href="#" target="_blank"> FAQs </a>  </li>
        <li> <a href="#" target="_blank"> Products </a>  </li>
        <li> <a href="#" target="_blank"> Blog </a>  </li>
      </ul>
    </div>
    <div class="footer-items">
      <h2>Shipping &amp; Returns</h2>
      <ul>
        <li> <a href="#" target="_blank"> Shipping Price &amp; Times</a>  </li>
        <li> <a href="#" target="_blank"> Return Policy </a>  </li>
        <li> <a href="#" target="_blank"> Coupons &amp; Deals </a>  </li>
      </ul>
    </div>
    <div class="footer-items footer-items-logo">
      <h2>Connect With Us</h2>
      <div class="footer-logo-container">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style>
:root {
  --primary-color:  #D5E5E4; /* green 100*/
  --secondary-color: #050D0C; /* green 900*/
  --tertiary-color:  #235F5A; /* green 600*/
  --quaternary-color: #173F3C; /* green 700*/
}

.footer-container {
  display: flex;
  justify-content: space-around;
  padding: 1rem;

  background-color: var(--tertiary-color);
  color: var(--primary-color);
  text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.25);
  }
.footer-items {
  text-align: justify;
}
.footer-items ul li a {
  text-decoration: none;
  color: var(--primary-color)
  }
.footer-items ul {
  padding: 0;
}
.footer-items ul li {
  list-style: none;
  }

.footer-items-logo {
  display: flex;
  flex-direction: column;
  text-align: center;
  width: 20%;;
}
.footer-logo-container {
  display: flex;
  justify-content: space-around;

}
.footer-items-logo img {
  object-fit: contain;
  width: 100%;
  max-width: 20%;
}

@media (max-width: 800px) {
  .footer-container {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .footer-items {
    flex-grow: 2;
  }
}
</style>