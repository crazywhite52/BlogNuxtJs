<template>
  <div>
    <b-container class="bg">
      <div class="center">
        <b-card no-body class="overflow-hidden" style="max-width: 100% ">
          <b-row no-gutters>
            <b-col sm="12" md="12" lg="12">
              <b-card-img
                src="https://assets.wallpapersin4k.org/uploads/2017/04/Wallpaper-Blogs-12.png"
                alt="Image"
                class="rounded-0"
                tag="article"
              ></b-card-img>
            </b-col>
            <b-col md="6" lg="12">
              <b-card-body title="Torkait Vue Nuxt.js">
                <h2 class="subtitle">torkait.it@gmail.com</h2>
                <b-card-text>
                  <nuxt-link to="/posts" class="button--grey">Users</nuxt-link>
                  <nuxt-link to="/admin" class="button--grey">Admin</nuxt-link>
                  <nuxt-link to="/login" class="button--grey">Login</nuxt-link>
                  
                </b-card-text>
              </b-card-body>
            </b-col>
          </b-row>
        </b-card>
      </div>
    </b-container>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style scoped>
.bg {
  background-color: #863d3d;
}
.center {
  margin: auto;
  max-width: 70vh;
  min-height: 10vh;
  min-width: 10vh;
  padding: 10px;
}
/* .container {
  margin: 0 auto;
  min-height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
} */

/* .title {
  font-family: 'Lucida Console', Courier, monospace;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
} */

.subtitle {
  font-weight: 300;
  font-size: 20px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
#Top {
  padding-top: 15px;
}
/* .links {
  padding-top: 15px;
} */
</style>
