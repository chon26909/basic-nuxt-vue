<template>
  <b-carousel
    id="carousel-1"
    v-model="slide"
    :interval="4000"
    controls
    indicators
    background="#ababab"
    img-width="1024"
    img-height="480"
    style="text-shadow: 1px 1px 2px #333"
    @sliding-start="onSlideStart"
    @sliding-end="onSlideEnd"
  >
    <div v-for="item in images" :key="item.caption">
      <b-carousel-slide :caption="item.caption" :img-src="item.img">
        <h1>{{ item.caption }}</h1>
      </b-carousel-slide>
    </div>
  </b-carousel>
</template>
<script>
export default {
  data() {
    return {
      images: [
        {
          caption: 'First slide',
          img: 'https://picsum.photos/1024/480/?image=52',
        },
        {
          caption: 'second slide',
          img: 'https://picsum.photos/1024/480/?image=54',
        },
        {
          caption: 'Thrid slide',
          img: 'https://picsum.photos/1024/480/?image=58',
        }
      ],
    }
  },
}
</script>
