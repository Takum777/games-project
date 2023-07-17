<template>
  <button class="nav-button">
    {{ buttonText }}
  </button>
</template>

<script>
export default {
  name: "NavButton",
  props: {
    buttonText: {
      type: String,
      required: true
    }
  }
}
</script>

<style>
button.nav-button {
  margin-left: 3%;
  font-size: 140%;
  letter-spacing: 1px;
  color: #ffffff;
  font-family: "Bebas Neue Regular";
  background: none;
  border: none;
  padding: 0;
  cursor: pointer;
  transition: color 0.3s, text-decoration-color 0.3s;
  text-decoration: none;
}

button.nav-button:hover {
  color: #2280ff;
  text-decoration-color: #2280ff;
  text-decoration: none; 
  border-bottom: 4px solid #2280ff; 
  padding-bottom: 8px;
}
</style>
