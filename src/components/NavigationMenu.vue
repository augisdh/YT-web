<template>
  <div>
    <div class="menu-bg" :class="{'active': burgerActive === true, 'inactive': burgerActive !== true}">
      <div class="menu-ctx">
        <div class="routes">
          <router-link to="/">Home</router-link>
          <router-link to="/about">About</router-link>
          <router-link to="/courses">Courses</router-link>
          <router-link to="/staff">Staff</router-link>
          <router-link to="/art-major">Art Major</router-link>
          <router-link to="/universities">Universities</router-link>
        </div>
      </div>
    </div>

    <div class="menu-bar nav-bar-position">
      <img @click="burgerClick" :class="{'active': burgerActive !== true, 'inactive': burgerActive === true}" src="./assets/contactform/burger-icon.png" alt="">
      <img @click="burgerClick" :class="{'active': burgerActive === true, 'inactive': burgerActive !== true}" src="./assets/contactform/x-icon-blue.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavigationMenu',
  data () {
    return {
      burgerActive: null
    }
  },
  methods: {
    burgerClick () {
      (this.burgerActive === null) ? this.burgerActive = true : this.burgerActive = !this.burgerActive
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.menu-bg {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.7);
  z-index: 5;
  display: flex;
  justify-content: flex-end;
}

  .menu-ctx {
    max-width: 850px;
    width: 100%;
    height: 100%;
    background: #fccd0f;
    margin-left: 20px;
    transition: all 0.3s;
  }

.menu-bar > img {
  width: 40px;
  height: 40px;
  cursor: pointer;
}

.inactive {
  display: none;
}
.active {
  display: flex;
}
</style>
