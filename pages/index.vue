<template>
  <div>

    <div style="max-height: 300px">
      <!--
    <b-carousel :autoplay="autoPlay">
      <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
        <section :class="`hero is-medium is-${carousel.color}`">
          <span class="image">
              <img :src="image(carousel.src)">
          </span>
        </section>
      </b-carousel-item>
    </b-carousel>
      -->
    </div>

    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
        </div>
        <div class="columns">
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
        </div>
        <div class="columns">
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
          <div class="column is-half">
            <div class="columns">
              <div class="column is-one-third">
                <img
                  src="https://images11.popmeh.ru/upload/img_cache/360/360dca32418be98bfc1013c4fdcd0125_fitted_800x3000.jpg"
                  width="100%">
              </div>
              <div class="column">Хорошие грузовики</div>
            </div>
          </div>
        </div>

      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column is-one-fifth">
            <img src="../assets/images/slide1.jpg">
          </div>
          <div class="column">28 доставлеенных грузов из 100!</div>
        </div>
        <div class="columns">
          <div class="column is-one-fifth">
            <img src="../assets/images/slide2.jpg">
          </div>
          <div class="column">Сытые водители!</div>
        </div>
        <div class="columns">
          <div class="column is-one-fifth">
            <img src="../assets/images/slide3.jpg">
          </div>
          <div class="column">Купленные полицейские на всех постах!</div>
        </div>
      </div>
    </section>

    <section class="section feedback">
      <div class="container">
        <div class="columns">
          <div class="column">
            <h2 class="title">
              Связаться с нами
            </h2>
          </div>
        </div>
        <div class="columns">
          <div class="column">
            <template>
              <section>
                <b-field label="Имя">
                  <b-input v-model="name"></b-input>
                </b-field>

                <b-field label="Телефон"
                         type="is-danger"
                         message="Телефон указан неверно">
                  <b-input type="phone"
                           value="890312312"
                           maxlength="30">
                  </b-input>
                </b-field>
              </section>
            </template>
          </div>
          <div class="column">
            <section>
              <b-field label="Сообщение">
                <b-input maxlength="200" type="textarea"></b-input>
              </b-field>
            </section>
          </div>
        </div>
        <div class="columns">
          <div class="column">
            <div class="buttons">
              <b-button type="is-success" outlined>Отправить</b-button>
            </div>
          </div>
        </div>

      </div>
    </section>


  </div>

</template>

<script>

export default {
  data () {
    return {
      autoPlay: false,
      carousels: [
        {text: 'Slide 1', src: 'slide1.jpg', color: 'primary'},
        {text: 'Slide 2', src: 'slide2.jpg', color: 'info'},
        {text: 'Slide 3', src: 'slide3.jpg', color: 'success'}
      ]
    }
  },

  methods: {
    image(src) {
      console.log(src)
      const fileName = src.toLowerCase();
      return require(`../assets/images/${fileName}`);
    }
  }
}
</script>
<style lang="scss">

  $carousel-min-height: '400px';

  img {
    display: block;
  }



  .title {
    color: #363636;
    font-size: 2rem;
    font-weight: 600;
    line-height: 1.125;
  }

  .feedback {
    background-color: #efefef;
  }

</style>
