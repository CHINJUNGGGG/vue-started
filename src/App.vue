<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link :to="{ name: 'profile', params: { username: 'mark2021' } }">Profile</router-link> |
    <router-link :to="
                      { 
                        name: 'product', 
                        params: 
                            { 
                              brand: 'Apple',
                              product: 'Apple watch series 7 45mm (Aluminium)',
                              price: '100$',
                              shop: 'Apple store in California, USA',
                              image: '../assets/aw7.jpeg',
                            } 
                      }">Product
    </router-link> 
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
