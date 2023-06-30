<template>
  <div>
    <div>
      <router-link to="/" class="nav-box-active">
        <div class="nav-outer-box-active">
          <span class="material-symbols-rounded"> home </span>
        </div>
        <b>Home</b>
      </router-link>
      <router-link to="" class="nav-box-inactive">
        <div class="nav-outer-box-active"></div>
        Einstellungen
      </router-link>
      <router-link to="" class="nav-box-inactive">
        <div class="nav-outer-box-active"></div>
        Statusübersicht
      </router-link>
    </div>
  </div>
</template>
<script setup lang="ts"></script>

<style>
.nav-outer-box-active {
  border-radius: 0.5rem;
  background: linear-gradient(228deg, #1daf36 0%, #95eb2c 100%);
  box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1);
  min-width: 2.25rem;
  min-height: 2.25rem;
  flex-shrink: 0;
  margin-right: 0.25rem;
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
