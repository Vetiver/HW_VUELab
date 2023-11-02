<script>
import { ref } from 'vue'
export default {
    setup(){

const arrow = ref(require('../../assets/images/arrow.png'))

return  { arrow }
    }
}
</script>

<template lang="">
    <section class="portfolio">
      <h3 class="portfolio__title">Портфолио</h3>

      <ul class="portfolio__sites">
        <li>
          <a
            class="portfolio__sites-item"
            href="https://github.com/Vetiver/HW_FastApi"
            target="_blank"
            rel="noreferrer"
          >
            FastAPI
            <img
              v-bind:src="arrow"
              class="portfolio__sites-item-arrow"
              alt="стрелка наверх-направо"
            />
          </a>
        </li>

        <li>
          <a
            class="portfolio__sites-item"
            href="https://github.com/Vetiver/goAPI"
            target="_blank"
            rel="noreferrer"
          >
            GoAPI
            <img
              v-bind:src="arrow"
              class="portfolio__sites-item-arrow"
              alt="стрелка наверх-направо"
            />
          </a>
        </li>

        <li>
          <a
            class="portfolio__sites-item portfolio__sites-item_application"
            href="https://github.com/Vetiver/algososh"
            target="_blank"
            rel="noreferrer"
          >
            Визуализация алгоритмов
            <img
              v-bind:src="arrow"
              class="portfolio__sites-item-arrow"
              alt="стрелка наверх-направо"
            />
          </a>
        </li>
      </ul>
    </section>
</template>
<style scoped>
    .portfolio {
  padding: 100px 0 87px;
  margin: 0 auto;
  max-width: 1140px;
}

.portfolio__title {
  max-width: 1140px;
  margin: 0 0 50px;
  color: #8b8b8b;
  font-size: 18px;
  font-weight: 400;
  line-height: 20px;
}

.portfolio__sites {
  list-style: none;
  margin: 19px auto 0;
  padding: 0 70px 0 0;
}

.portfolio__sites-item {
  color: #FFF;
  width: 1140px;
  margin-bottom: 20px;
  padding-bottom: 19px;
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #424242;
  font-size: 30px;
  line-height: 50px;
  letter-spacing: -1.2px;
  text-decoration: none;
}

.portfolio__sites-item_application {
  border-bottom: none;
}

.portfolio__sites-item-arrow {
  width: 27px;
  height: 27px;
  margin-right: 5px;
}

/* ------------------------------------ */
@media screen and (max-width: 1279px) {
  .portfolio {
    max-width: 668px;
    padding: 90px 0 52px ;
  }

  .portfolio__sites {
    margin: 50px auto 0;
    padding: 0;
  }

  .portfolio__sites-item {
    width: 668px;
    font-size: 28px;
    line-height: 50px;
    letter-spacing: -1.12px;
  }
}

@media screen and (max-width: 767px) {
  .portfolio {
    max-width: 292px;
    padding: 70px 0 32px;
  }

  .portfolio__title {
    margin: 0 0 40px;
    text-align: start;
    font-size: 14px;
    line-height: 20px;
  }

  .portfolio__sites {
    margin: 0 auto;
    padding: 0;
  }

  .portfolio__sites-item {
    width: 292px;
    font-size: 18px;
    line-height: 28px;
    letter-spacing: -0.72px;
  }

  .portfolio__sites-item-arrow {
    width: 10px;
    height: 10px;
    margin-top: 8px;
  }
}
</style>