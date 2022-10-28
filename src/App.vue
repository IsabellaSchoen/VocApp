<template>
  <nav class="navigation-bar">
    <div class="home-class">
          <router-link to="/">
            <i class="fa fa-home fa-2x" aria-hidden="true"></i>
          </router-link>
      </div>
      <div class="settings-class">
        <router-link to="/settings">
          <i class="fa fa-cog fa-2x" aria-hidden="true"></i>
        </router-link>
      </div>
  </nav>
  <router-view />
</template>

<style>
#app {
  font-family: 'Meridien', sans-serif;
  text-align: center;
  background-image: url('./assets/background_pic_one.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
.navigation-bar {
  display: grid;
  gap: 400px;
  padding: 0px;
  background-color: rgba(189, 189, 189, 0.815);
  grid-template-columns: auto auto;
}

.home-class {
  padding: 20px 0;
  font-size: 20px;
}

.home-class > a {
  text-decoration: none;
  color: black;
}

.settings-class {
  padding: 20px 0;
  font-size: 20px;
}

.settings-class > a {
  text-decoration: none;
  color: black;
}
</style>

#LJUoCTHII%#wA&G