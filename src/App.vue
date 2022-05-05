<template>
  <div class="BodyBasic">
    <HeaDer></HeaDer>
    <div class="SelectButton">
      <nav>
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </nav>
      <router-view/>
    </div>
    <FooTer></FooTer>
  </div>
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

.SelectButton{
  margin-top: 5rem;
}

.BodyBasic{
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  background: linear-gradient(-45deg, #ffffff, #ccccff);
  background-size: 400% 400%;
  -webkit-animation: Gradient 20s ease infinite;
  -moz-animation: Gradient 20s ease infinite;
  animation: Gradient 20s ease infinite;
}
@-webkit-keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}
@-moz-keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}
@keyframes Gradient {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}

</style>
<script>
import FooTer from '@/components/FooterAndHeader/Footer'
import HeaDer from '@/components/FooterAndHeader/Header'
export default {
  components: {
    HeaDer,
    FooTer
  }
}
</script>
