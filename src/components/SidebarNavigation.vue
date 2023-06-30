<template>
  <div>
    <div>
      <router-link to="/" class="nav-box-active">
        <div class="nav-outer-box-active">
          <span class="material-symbols-rounded">home</span>
        </div>
        <b>Home</b>
      </router-link>
      <router-link to="" class="nav-box-inactive">
        <div class="nav-outer-box-inactive">
          <span class="material-symbols-rounded">settings</span>
        </div>
        Einstellungen
      </router-link>
      <router-link to="" class="nav-box-inactive">
        <div class="nav-outer-box-inactive">
          <span class="material-symbols-rounded">help</span>
        </div>
        Statusübersicht
      </router-link>
    </div>
  </div>
</template>
<script setup lang="ts"></script>

<style lang="scss">
.nav-outer-box-active {
  border-radius: 0.5rem;
  background: linear-gradient(228deg, #1daf36 0%, #95eb2c 100%);
  box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1);
  padding: 0.5rem;
  flex-shrink: 0;
  margin-right: 1rem;

  span {
    color: white;
  }
}

.nav-outer-box-inactive {
  border-radius: 0.5rem;
  background: #fff;
  box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1);
  padding: 0.5rem;
  flex-shrink: 0;
  margin-right: 1rem;
}

.nav-box-inactive {
  color: #344767;
  display: flex;
  align-items: center;
  font-size: large;
  text-decoration: none;
  padding: 0.6rem 1rem;
}

.nav-box-active {
  color: #344767;
  display: flex;
  align-items: center;
  font-size: x-large;
  text-decoration: none;
  padding: 0.6rem 1rem;
  border-radius: 0.625rem;
  background: #fff;
  box-shadow: 0px 20px 20px 0px rgba(0, 0, 0, 0.05);
}
</style>
