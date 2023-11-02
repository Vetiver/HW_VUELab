<script>
import { ref } from 'vue'
export default {
    setup(){

const pic = ref(require('../../assets/images/logo.jpg'))

return  { pic }
}  
}
</script>

<template lang="">
       <header class='header'>
        <img class='logo' v-bind:src="pic" alt="логотип">
    </header>
</template>

<style scoped>
    .header {
        padding-top: 18px;
        padding-bottom: 18px;
  padding-right: 70px;
  padding-left: 70px;
  background-color: #073042;
  display: flex;
  position: relative;

}

.logo {
    width: 200px;
    height: 200px;
    border-radius: 390px;
}



/* ------------------------------------ */

@media screen and (max-width: 768px) {
  .header {
    padding: 0 30px;
  }


}

@media screen and (max-width: 400px) {
  .header {
    padding: 0 14px;
  }


}
</style>