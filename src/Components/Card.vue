<template>
  <div>
    <img alt="Vue logo" width="100%" height="50" src="../assets/logoh.png">
    <card-swipe>
      <card-swipe-item>
      <div
        class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
      >45</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >2</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >3</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >4</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >5</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >6</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >7</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >8</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >9</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >10</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >11</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >12</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >13</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >14</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >15</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >16</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >17</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >18</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #ffaa00 0%, #ff8800 100%);"
        >19</div>
      </card-swipe-item>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #add0f8 0%, #5ca2f8 100%);"
        >20</div>
      </card-swipe-item>
    </card-swipe>
  </div>
</template>

<script>
import { CardSwipe, CardSwipeItem } from "@eshengsky/vue-card-swipe";

export default {
name: 'Card',
  components: {
    CardSwipe,
    CardSwipeItem
  },
  methods: {
  redirect() {
    location.href = "https://m.lvmama.com";
  },
  onResume(currentIndex) {
    this.evtMessage = `#${currentIndex} resumed!`;
  },
  onChange(lastIndex, currentIndex) {
    this.evtMessage = `#${lastIndex} -> #${currentIndex}`;
  }
}
};
</script>

<style>
body {
  max-width: 375px;
  margin: 50px auto;
}

.detail-wrap {
  display: block;
  height: 100%;
  border-radius: 5px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.detail-wrap h5 {
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  padding: 0 15px;
  display: -webkit-box;
  overflow: hidden;
  text-overflow: ellipsis;
  -webkit-box-orient: vertical;
  word-break: break-all;
  font-size: 16px;
  line-height: 20px;
  color: #fff;
  -webkit-line-clamp: 2;
  max-height: 38px;
  font-weight: bold;
  margin-bottom: 10px;
  text-shadow: 0px 0px 4px #333;
}

.color-card {
  height: 500px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 8px;
  color: #fff;
}

.msg {
  font-size: 14px;
  margin: 10px 0;
  color: #555;
}
</style>
