<script>
import { ref } from 'vue'
export default {
    setup(){

const uzor = ref(require('../../assets/images/uzor.png'))

return  { uzor }
    }
};
</script>

<template lang="">
  <section class="promo">
    <h1 class="promo__title">
      Сайт визитка студента МТУСИ на VUE.js
    </h1>
    <img v-bind:src="uzor" class="promo__uzor" alt="узор" />
  </section>
</template>
<style scoped>
.promo {
  display: flex;
  flex-direction: column;

  background-color: #073042;
  padding: 50px 70px 60px 70px;
  margin: 0 auto;
}

.promo__title {  
  margin: 0;
  padding: 0;
  max-width: 519px;
  color: #FFF;
  text-align: left;
  font-size: 40px;
  font-weight: 400;
  line-height: 52px;
  letter-spacing: -1.6px;
}

.promo__uzor {
  width: 722px;
  height: 244px;
  margin-top: 102px;
  display: flex;
  align-self: flex-end;
}


@media screen and (max-width: 1279px) {
  .promo {    
    padding: 300px 44px 70px 44px;
  }

  .promo__title {    
    margin: 0 0 40px 80px;    

    text-align: center;
    line-height: 52px;
    letter-spacing: -1.6px;
  }

  .promo__uzor {
    width: 680px;
    height: 230px;    
  }

}

/* --------------------------------- */
@media screen and (max-width: 767px) {

  .promo {
    padding: 183px 0 40px 0;
  }


  .promo__uzor {
    margin: 60px 0 0 0;    
    object-fit: cover;
  }

  .promo__title {    
    font-size: 31px;
    line-height: 39px;
    letter-spacing: -1.24px;
  }
}

@media screen and (max-width: 320px) {
  .promo__uzor {
    margin: 60px 0 0 0;
    height: 230px;
    width: 320px;
    object-fit: cover;
  }

  .promo__title {
    margin: 0;
    font-size: 31px;
    line-height: 39px;
    letter-spacing: -1.24px;
  }
}
</style>
