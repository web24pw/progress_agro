<template>
  <div>
    <nuxt/>
    <footer class="footer">
      <div class="container">
        <div class="columns">
          <div class="column">
            <h3 class="footer_title">О компании</h3>
            <p class="footer_paragraph_accent">Наименование</p>
            <p class="footer_paragraph">ООО «Прогресс Агро»</p>
            <p class="footer_paragraph_accent">Директор</p>
            <p class="footer_paragraph">Курталидис Михаил Сергеевич</p>
          </div>
          <div class="column">
            <h3 class="footer_title">Контакты</h3>
            <p class="footer_paragraph_accent">Адрес</p>
            <p class="footer_paragraph">117279, Москва, ул. Миклухо-Маклая, 34 Э0
              пом. IV к37 оф 265</p>
            <p class="footer_paragraph_accent">Телефон</p>
            <p class="footer_paragraph">+7 916 268-81-87</p>
            <p class="footer_paragraph_accent">E-mail</p>
            <p class="footer_paragraph">info@progress-agro.com.ru</p>
          </div>
          <div class="column">
            <h3 class="footer_title">Реквизиты</h3>
            <div class="footer__block">
              <div class="footer__block_accent">ИНН/КПП</div>
              <div class="footer__block_paragraph">7728483081/ 772801001</div>
            </div>
            <div class="footer__block">
              <div class="footer__block_accent">ОГРН</div>
              <div class="footer__block_paragraph">1197746497629</div>
            </div>
            <div class="footer__block">
              <div class="footer__block_accent">Расчётный счет</div>
              <div class="footer__block_paragraph">40702810702730003599</div>
            </div>
            <div class="footer__block">
              <div class="footer__block_accent">Корреспондентский счет</div>
              <div class="footer__block_paragraph">30101810200000000593</div>
            </div>
            <div class="footer__block">
              <div class="footer__block_accent">БИК банка</div>
              <div class="footer__block_paragraph">044525593</div>
            </div>
            <div class="footer__block">
              <div class="footer__block_accent">Банк</div>
              <div class="footer__block_paragraph">АО "АЛЬФА-БАНК"</div>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
  html {
    font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *, *:before, *:after {
    box-sizing: border-box;
    margin: 0;
  }

  .button--green {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
  }

  .button--green:hover {
    color: #fff;
    background-color: #3b8070;
  }

  .button--grey {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
  }

  .button--grey:hover {
    color: #fff;
    background-color: #35495e;
  }

  .footer_title{
    color: #363636;
    font-size: 1.25rem;
    font-weight: 600;
    margin-bottom: 1rem;
  }

  .footer_paragraph_accent{
    color: #363636;
    font-size: 1em;
    font-weight: 600;
    margin-bottom: .25rem;
    margin-top: .5rem;
  }
  .footer__block{
    display: flex;
    margin-bottom: .25rem;
    margin-top: .5rem;
  }
  .footer__block_accent{
    color: #363636;
    font-size: 1em;
    font-weight: 600;
  }
  .footer__block_paragraph{
    margin-left: .5rem;
  }
</style>

