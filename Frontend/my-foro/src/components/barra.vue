<template>
  <div class="w-100">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <h4 style="background-color: white;">{{ user.nombre + " " + user.apellido }}</h4>
      </div>
    </nav>
  </div>
</template>
<script>
export default {
  name: "barra",
  data() {
    return {
      user: null,
    };
  },
  created: function () {
    this.user = JSON.parse(localStorage.getItem("user"));
  },
};
</script>