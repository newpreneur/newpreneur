<template>
  <div id="app">
    <card-swipe>
      <card-swipe-item>
        <div
          class="color-card"
          style="background-image: linear-gradient(to right, #fe686c 0%, #fe3c71 100%)"
        >1</div>
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
    </card-swipe>
  </div>
</template>

<script>
import { CardSwipe, CardSwipeItem } from "@eshengsky/vue-card-swipe";
export default {
name: 'App',
  components: {
    CardSwipe,
    CardSwipeItem
  }
};
</script>

<style>
body {
  max-width: 375px;
  margin: 10px auto;
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

  font-size: 36px;
}

.msg {
  font-size: 14px;
  margin: 10px 0;
  color: #555;
}
</style>
