<template>
  <div class="main_container">
    <div class="main_img_bg">
      <div class="main_img"></div>
    </div>
    <div class="main_content">
      <div class="aff">
        <a target="_blank" href="https://www.millipiyangoonline.com/">
          <div class="aff_link aff_link_milli"></div>
        </a>
        <a
          target="_blank"
          href="https://refpaiozdg.top/L?tag=d_1858619m_30577c_&site=1858619&ad=30577"
        >
          <div class="aff_link aff_link_megapari"></div>
        </a>
      </div>
      <div class="content_container">
        <div class="top_container">
          <div class="title">Megapari Milli Piyango</div>
          <a
            target="_blank"
            href="https://refpaiozdg.top/L?tag=d_1858619m_30577c_&site=1858619&ad=30577"
          >
            <div class="btn">Kayıt Olun</div>
          </a>
        </div>
        <div class="middle_container">
          <div class="title-small">Nasıl katılım sağlanır?</div>
          <ol type="">
            <li class="text">
              Megapari web sitesine kaydolun veya giriş yapın.
            </li>
            <a target="_blank" href="https://forms.gle/xXrhjeGVFi3oEZap6">
              <div class="btn btn-list">Katılın</div>
            </a>
            <li class="text">
              Promosyona katılımınızı onaylamak için formu doldurun. 01.12.2022
              - 31.12.2022 tarihleri ​​arasında herhangi bir spor etkinliğine
              veya kumarhaneye 100₺'den başlayan bahisler yapın. Ne kadar çok
              bahis ₺200.000'lik ödül havuzundan pay alma şansınız o kadar
              yüksek!
            </li>
            <li class="text">Ödül havuzu 6 aşamadan oluşmaktadır:</li>
            <div class="list">
              <div
                v-for="(el, id) in Object.keys(levelList)"
                :key="id"
                class="list_el"
              >
                • {{ el }} - {{ levelList[el] }}
              </div>
            </div>
          </ol>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    const levelList = {
      'Level 1': '20 000 ₺',
      'Level 2': '20 000 ₺',
      'Level 3': '50 000 ₺',
      'Level 4': '45 000 ₺',
      'Level 5': '40 000 ₺',
      'Level 6': '25 000 ₺',
    };
    return {
      levelList,
    };
  },
};
</script>

<style lang="sass" scoped>
.main_container
  position: relative
  background: radial-gradient(69.95% 279.79% at 69.95% 17.24%, rgba(255, 255, 255, 0.2) 0%, rgba(0, 0, 0, 0.2) 100%), #3F8DD6
  width: 100vw
  min-height: 1440px
  overflow-x: hidden
  background-image: url('./icons/main_bg.png')
  background-position: bottom -120px right 0
  background-size: contain
  background-repeat: no-repeat
  @media (max-width: 421px)
    padding-bottom: 40px
    background-position: bottom -0px right 0
    background-image: url('./icons/main_bg_mobile.png')
  .main_img_bg
    position: absolute
    top: 0
    left: 50%
    width: 955px
    height: 785px
    background-position: center
    background-size: contain
    background-repeat: no-repeat
    background-image: url('./icons/main_img.png')
    @media (max-width: 421px)
      top: 200px
      left: -10%
      width: 476px
      height: 400px
    .main_img
      height: 100%
      width: 100%
      background: #AAAAAA
      background-image: url('./icons/Ellipse_1.png')
      mix-blend-mode: overlay
      filter: blur(75px)
      transform: rotate(5.18deg)
      background-position: center
      background-size: contain
      background-repeat: no-repeat
  .main_content
    max-width: 1300px
    margin: 0 auto
    margin-top: 60px
    @media (max-width: 421px)
      max-width: 360px
      margin-top: 20px
    .aff
      display: flex
      flex-direction: row
      gap: 25px
      @media (max-width: 421px)
        gap: 20px
        align-items: center
        justify-content: space-evenly
      .aff_link
        background: #FFFFFF
        border-radius: 32px
        height: 92px
        width: 218px
        background-position: center
        background-size: initial
        background-repeat: no-repeat
        @media (max-width: 421px)
          width: 150px
          height: 64px
          background-size: contain
        &_milli
          background-image: url('/src/assets/milli_logo.svg')
          @media (max-width: 421px)
            background-size: 115px
        &_megapari
          background-image: url('/src/assets/megapari_logo.svg')
    .content_container
      @media (max-width: 421px)
        width: 360px
        display: flex
        flex-direction: column
        align-items: center
      .top_container
        display: flex
        flex-direction: column
        gap: 60px
        margin-top: 100px
        margin-bottom: 100px
        @media (max-width: 421px)
          margin-top: 40px
          width: 360px
          align-items: center
        .title
          font-weight: 800
          font-size: 74px
          line-height: 120%
          color: #FFFFFF
          max-width: 550px
          @media (max-width: 421px)
            padding-bottom: 320px
            font-weight: 800
            font-size: 38px
            line-height: 120%
            max-width: 278px
            align-self: flex-start
        .btn
          display: flex
          align-items: center
          justify-content: center
          width: 400px
          height: 80px
          background: #FFFFFF
          box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
          border-radius: 73px
          font-weight: 800
          font-size: 36px
          line-height: 100%
          color: #3E7DB7
          cursor: pointer
          @media (max-width: 421px)
            width: 260px
            height: 62px
            font-size: 28px
          &:hover
            background: linear-gradient(0deg, #406D98, #406D98), #FFFFFF
            border: 2px solid #FFFFFF
            box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
            border-radius: 73px
            color: white
          &::active
            background: linear-gradient(0deg, #406D98, #406D98), #FFFFFF
            border: 2px solid #FFFFFF
            box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
            border-radius: 73px
            color: white
      .middle_container
        .title-small
          font-weight: 700
          font-size: 28px
          line-height: 100%
          color: #FFFFFF
          margin-bottom: 40px
          @media (max-width: 421px)
            font-size: 24px
        .text
          font-weight: 500
          font-size: 24px
          color: #FFFFFF
          line-height: 130%
          max-width: 650px
          @media (max-width: 421px)
            font-size: 16px
            line-height: 19.2px
        .btn
          display: flex
          align-items: center
          justify-content: center
          width: 400px
          height: 80px
          background: #FFFFFF
          box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
          border-radius: 73px
          font-weight: 800
          font-size: 36px
          line-height: 100%
          color: #3E7DB7
          margin-top: 35px
          margin-bottom: 35px
          cursor: pointer
          @media (max-width: 421px)
            width: 260px
            height: 62px
            font-size: 28px
          &:hover
            background: linear-gradient(0deg, #406D98, #406D98), #FFFFFF
            border: 2px solid #FFFFFF
            box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
            border-radius: 73px
            color: white
          &::active
            background: linear-gradient(0deg, #406D98, #406D98), #FFFFFF
            border: 2px solid #FFFFFF
            box-shadow: 0px 20px 50px rgba(0, 0, 0, 0.1)
            border-radius: 73px
            color: white
          &-list
            margin-left: -35px
            @media (max-width: 421px)
              margin-left: 2%
        .list
          font-weight: 500
          font-size: 24px
          line-height: 180%
          color: #FFFFFF
          margin-left: 20px
          @media (max-width: 421px)
            font-size: 16px
@media (max-width: 421px)
  .aff_link
    width: 150px
    height: 64px
</style>
