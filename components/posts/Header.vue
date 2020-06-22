<template>
  <div style="margin-top: 5px;">
    <b-row>
      <b-col>
        <b-carousel id="slider" controls indicators>
          <div v-for="(item,i) in items" :key="i">
            <b-carousel-slide :caption="item.caption" :text="item.text" :img-src="item.image"></b-carousel-slide>
          </div>
        </b-carousel>
      </b-col>
    </b-row>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          caption: 'ท่องเที่ยว',
          image: require('@/assets/image/p4.jpg'),
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.'
        },
        {
          caption: 'ท่องเที่ยว',
          image: require('@/assets/image/p5.jpg'),
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.'
        },
        {
          caption: 'ท่องเที่ยว',
          image: require('@/assets/image/p1.jpg'),
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.'
        },
        {
          caption: 'ท่องเที่ยวธรรมชาติ',
          image: require('@/assets/image/p2.jpg'),
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.'
        },
        {
          caption: 'ท่องเที่ยว',
          image: require('@/assets/image/p3.jpg'),
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.'
        }
      ]
    }
  }
}
</script>