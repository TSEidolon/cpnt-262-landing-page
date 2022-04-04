# CPNT-262 Assignment 2 - Vue/Nuxt Landing Page
## By: Edgar Caballero

Live Netlify Site:  [ScalesEmporium](https://majestic-horse-ca27b9.netlify.app/)

Troubleshooting: 
 - Made use of the addEventListener JS function for the reposponsive navigation menu.
 - Since I was using Vue, I changed the `addEventListener` to a `v-on` for easier and more concise vue components

 Went from this:
 ```
 <script setup>
  import {onMounted} from 'vue'
onMounted (() => {
  const toggleButton = document.getElementsByClassName('toggle-button')[0];
  const navbarLinks = document.getElementsByClassName('navbar-links')[0];
  toggleButton.addEventListener('click', ()=> {
  navbarLinks.classList.toggle('active')
</script>
 ```
To This:
```
<script setup>
function ShowMenu () {
    const navbarLinks = document.getElementsByClassName('navbar-links')[0];
    navbarLinks.classList.toggle('active')
  }
</script>
```
- Attempted to add Font Awesome Icons to Vue by following the "[Font Awesome with Vue JS Website](https://fontawesome.com/docs/web/use-with/vue/)"
 - According to [Suboptimal Engineer: How to Add Font Awesome Icons in Vue 3](https://www.youtube.com/watch?v=MoDIpTuRWfM&t=704s), apparently `npm i --save @fortawesome/vue-fontawesome@latest` does not work for vue3 and I had to use `npm i --save @fortawesome/vue-fontawesome@prerelease` instead.



### Attributions:

 - [CSS Wavy Background Tutorial ](https://www.youtube.com/watch?v=0QTzTOJCzLY)

 - Images:
    - [green tree python - image by David Clode](https://unsplash.com/photos/5uU8HSpfwkI)
    - [fighting fish - image by Worachat Sodsri](https://unsplash.com/photos/nCz_ZgnbtaE)
    - [striped tiger butterfly - image by Sonika Agarwal](https://unsplash.com/photos/WBPcT5DC8wo)
    - [reptile - image by Linus Mimietz](https://unsplash.com/photos/7xm5J9FbZmw)
    - [snake - image by James Wainscoat](https://unsplash.com/photos/97UtyhmVjr4)
    - [fish - image by Claudio Guglieri](https://unsplash.com/photos/K2RH1QZdLF4)