<script setup>
import axios from 'axios';
// request for a user with a given id
axios.get('/user?ID=12345')
  .then(function (response) {
    // handle success
    console.log(response);
  })
  .catch(function (error) {
    // handle error
    console.log(error);
  })
  .finally(function () {
    // always executed
  });
// post request


</script>

<template>
    &nbsp;
</template>

<style scoped>


</style> 
