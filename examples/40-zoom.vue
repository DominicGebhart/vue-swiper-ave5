<template>
  <md-card>
    <md-card-actions>
      <div class="md-subhead">
        <span>Zoom</span>
        <span>（</span>
        <span>变焦、点击放大</span>
        <span>）</span>
      </div>
      <md-button
        class="md-icon-button"
        target="_blank"
        href="https://github.com/DarkRiDDeR/vue-swiper-ave5/blob/master/examples/40-zoom.vue"
      >
        <md-icon>code</md-icon>
      </md-button>
    </md-card-actions>
    <md-card-media>
      <!-- swiper -->
      <swiper :options="swiperOption">
        <swiper-slide>
          <div class="swiper-zoom-container">
            <img src="/static/images/surmon-6.jpg">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="swiper-zoom-container">
            <img src="/static/images/surmon-1.jpg">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="swiper-zoom-container">
            <img src="/static/images/surmon-3.jpg">
          </div>
        </swiper-slide>
        <div
          class="swiper-pagination swiper-pagination-white"
          slot="pagination"
        />
        <div
          class="swiper-button-prev"
          slot="button-prev"
        />
        <div
          class="swiper-button-next"
          slot="button-next"
        />
      </swiper>
    </md-card-media>
  </md-card>
</template>

<script>
  export default {
    data() {
      return {
        swiperOption: {
          zoom: true,
          pagination: {
            el: '.swiper-pagination'
          },
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
          }
        }
      }
    }
  }
</script>
