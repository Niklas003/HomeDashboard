<template>
  <div class="flex">
    <div>
      <router-link to="/" class="nav-box active">
        <div class="nav-inner-box">
          <span class="material-symbols-rounded larger">home</span>
        </div>
        <b>Home</b>
      </router-link>
      <router-link to="/settings" class="nav-box">
        <div class="nav-inner-box inactive">
          <span class="material-symbols-rounded">settings</span>
        </div>
        Einstellungen
      </router-link>
      <router-link to="/status" class="nav-box">
        <div class="nav-inner-box inactive">
          <span class="material-symbols-rounded">help</span>
        </div>
        Statusübersicht
      </router-link>
    </div>
    <div class="vertical-line"></div>
  </div>
</template>
<script setup lang="ts">
import router from "@/router";

const currentRoute = router.currentRoute;
console.log(currentRoute); /* printing it for future use */
</script>

<style lang="scss">
.flex {
  display: flex;
}

.larger {
  font-size: larger;
}

.nav-inner-box {
  border-radius: 0.5rem;
  background: linear-gradient(228deg, #1daf36 0%, #95eb2c 100%);
  box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1);
  padding: 0.5rem 0.5rem 0.3rem 0.5rem;
  margin-right: 1rem;

  span {
    color: white;
  }

  &.inactive {
    background: #fff;
    box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1);

    span {
      color: #344767;
    }
  }
}

.nav-box {
  margin: 0.55rem 0;
  color: #344767;
  display: flex;
  align-items: center;
  font-size: large;
  font-weight: 300;
  text-decoration: none;
  padding: 0.6rem 1rem;

  &.active {
    font-weight: 600;
    font-size: x-large;
    text-decoration: none;
    padding: 0.6rem 1rem;
    border-radius: 0.625rem;
    background: #fff;
    box-shadow: 0px 20px 20px 0px rgba(0, 0, 0, 0.05);
  }
}

.vertical-line {
  margin-left: 3rem;
  border-right: 0.0625rem solid rgba(0, 0, 0, 0.15);
  height: 13rem;
}
</style>
