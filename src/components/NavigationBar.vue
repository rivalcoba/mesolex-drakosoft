<template>
  <nav>
    <router-link to="/">LOGO</router-link>
    <div class="dropdown">
      <button class="dropbtn">
        {{ $t('byTopic') }}
        <i class="fa fa-caret-down"></i>
      </button>
      <div class="dropdown-content">
        <div class="header">
          <h2>{{ $t('dictionaries') }}</h2>
        </div>
        <div class="row">
          <div class="column">
            <h3>Maya</h3>
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
          <div class="column">
            <h3>Mixteco</h3>
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
        </div>
      </div>
    </div>
    <router-link to="/about">About</router-link>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  overflow: hidden;
  background-color: #333;
  font-family: Arial, Helvetica, sans-serif;
}

nav a {
  float: left;
  font-size: 16px;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.column a {
  float: none;
  color: black;
  padding: 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;
  border: none;
  outline: none;
  color: white;
  padding: 14px 16px;
  background-color: inherit;
  font: inherit;
  margin: 0;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  width: 100%;
  left: 0;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content .header {
  background: rgb(6, 89, 138);
  padding: 16px;
  color: white;
}

.dropdown:hover .dropdown-content {
  display: block;
  margin: 0px 10px;
}

.column {
  float: left;
  width: 50%;
  padding: 10px;
  background-color: #ccc;
  height: 250px;
}
</style>
<i18n>
{
  "en": {
    "byTopic": "By Topic",
    "dictionaries": "Dictionaries",
    "hello": "Hello i18n in SFC!"
  },
  "es":{
    "byTopic": "Por Tema",
    "dictionaries": "Diccionarios",
    "hello": "Hola i18n en Componente de Archivo!"
  }
}
</i18n>
