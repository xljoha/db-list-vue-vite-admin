<template>
<div class="navigation_wrapper">
  <div class="navbar navbar-dark bg-primary navbar-expand-xl">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">
        <span class="logo"><img :src="'/img/gub-textlogo-en.svg'" alt="logo"></span> | Databases Admin
      </a>
      <button class="navbar-toggler" type="button" 
              data-bs-toggle="collapse" data-bs-target="#navbarNav"
              aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link :to="{name: 'home'}" class="nav-link">Home</router-link>
          </li>
          <li class="nav-item" >
            <router-link :to="{name: 'index'}" class="nav-link">Topics</router-link>
          </li>
          <li class="nav-item" >
            <router-link :to="{name: 'mediatypeindex'}" class="nav-link">Mediatypes</router-link>
          </li>
          <li class="nav-item" >
            <router-link :to="{name: 'publisherindex'}" class="nav-link">Publishers</router-link>
          </li>
        </ul>
      </div>
    </div>
  </div>
</div>
</template>

<script>

export default {
  components: {
  },
  setup() {

  }
}
</script>

<style lang="scss" >
.navigation_wrapper {
  .navbar {
    margin-bottom: 20px;
    .nav-item {
      a {
        &:hover, &:focus {
            background-color: transparent;
          
        }
        &.router-link-active {
          background: transparent;
          border-bottom: 2px solid white;
        }
      }
    }
  }

}
</style>