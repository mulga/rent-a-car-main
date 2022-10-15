<template>
  <div class="content text-center">
    <slot></slot>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line
name:"Auth"
}
</script>

<style scoped>
  body {
    height: 100vh;
    width: 100%;
    display: flex;
    margin-top: 5rem;
  }
</style>
<style>
  .form-signin {
    width: 100%;
    max-width: 330px;
    padding: 15px;
    margin: auto;
    text-align: center;
     
  }
  .form-signin .checkbox {
    font-weight: 400;
  }
  .form-signin .form-control {
    position: relative;
    box-sizing: border-box;
    height: auto;
    padding: 10px;
    font-size: 16px;
  }
  .form-signin .form-control:focus {
    z-index: 2;
  }
  .form-signin input {
    margin-bottom: 10px;
     
  }
   
</style>