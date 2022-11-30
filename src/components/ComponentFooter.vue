<template>
  <div>
    <footer>
      <div class="title">
        Copyright © 2019-2022 «Megapari»
        <br />
        All rights reserved and protected by law.
      </div>
      <div class="text">
        megapari.com (http://megapari.com/) is owned and operated by Vdsoft &
        Script Development N.V. as a License Holder (Curacao license No.
        365/JAZ). Vdsoft Development Kft. (reg. number 01-09-397173) provides
        processing service on the website as a Billing Agent and with a
        registered office located at Vaci Street, 134/C. 5., 1134, Budapest,
        Hungary. Galaxsys Tech kft. (reg. number 13-09-217371) provides
        processing service on the website as a Billing Agent and with a
        registered office located at Cehmester utca 22., 2013, Pomaz, Hungary.
        All rights reserved and protected by law.
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style lang="sass" scoped>
footer
  display: flex
  flex-direction: column
  align-items: center
  justify-content: flex-start
  gap: 20px
  background: radial-gradient(69.95% 279.79% at 69.95% 17.24%, rgba(255, 255, 255, 0.2) 0%, rgba(0, 0, 0, 0.2) 100%), #3F8DD6
  padding: 85px
  @media (max-width: 421px)
    padding: 20px
  .title
    font-weight: 500
    font-size: 20px
    line-height: 122.52%
    text-align: center
    color: #FFFFFF
    max-width: 395px
    @media (max-width: 421px)
      font-size: 16px
      max-width: 309px
  .text
    font-weight: 300
    font-size: 20px
    line-height: 122.52%
    letter-spacing: 0.03em
    color: #FFFFFF
    max-width: 1069px
    @media (max-width: 421px)
      font-size: 12px
      letter-spacing: 0.03em
      max-width: 321px
</style>
