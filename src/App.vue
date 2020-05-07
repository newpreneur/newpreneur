<template>
  <div id="app">
  <div class="chat_area">
      <Card/>
    <div class = "chat_input">
    <input type="text" name="message" placeholder=" enter message here  and press Enter..."/>
    </div>
  </div>
    </div>
</template>

<script>
import Card from './Components/Card';
export default {
name: 'App',
components: {
 Card
},
};
</script>

<style>
  * {
     font-family: 'Open Sans', sans-serif;
   font-size : 16px;
    line-height : 1.5rem;
    color : #525c65;
    font-smooth: always;
    text-decoration : none;
  }
  body {
    background-size: cover;
  }
  #app {
    height : 100vh;
    display:flex;
    align-items: center;
    justify-content : space-around;
  }
  .chat_area {
    width : 400px;
    height : 700px;
    background : #fff;
    align-self : center;
    box-shadow : 8px 10px 20px 0px rgba(46,61,73,0.15);
    border-radius : 30px;
  position: relative;
    border : 5px solid rgba(0,0,0,0.2);


  }
  .chat_area .chat_input {
    position : absolute;
    bottom : 0;
    width : 100%;
    height : 50px;
    padding : 20px 0 20px 0;
    background:#FFEB3B;
    display : flex;
    justify-content : center;
    align-items: center;
    border-bottom-left-radius : 25px;
    border-bottom-right-radius : 25px;
    border-top : 5px solid #FDD835;
  }
  .chat_area .chat_input input {
    width : 80%;
    height : 40px;
    border : 1px solid transparent;
    box-shadow : 8px 10px 20px 0px rgba(61,61,61,0.5);
    padding : 10px;
    text-align : center;
    border-radius : 50px;
    text-transform : uppercase;
    font-size : 10px;
    letter-spacing : 2px;
  }
  .chat_area .conversation {
    width : 85%;
    margin : 0 auto;
    padding : 25px;
    margin-top : 20px;
    height : 620px;
    scrollbar-base-color: #fff;
    scrollbar-face-color: #dadada;
    scrollbar-3dlight-color: #fff;
    scrollbar-highlight-color: #fff;
    scrollbar-track-color: #fff;
    scrollbar-arrow-color: #fff;
    scrollbar-shadow-color: #fff;
    scrollbar-dark-shadow-color: #fff;




  }
  .message_bubble {
    text-transform : uppercase;
    display : flex;
    flex-direction : column;


  }
  .message_bubble .content .author , .message_bubble .content .message {
    font-size : 12px;
    letter-spacing : 2px;
  }

  .message_bubble .content {

    display : flex;
    padding:5px;
    margin-top : 5px;
    align-items : flex-start;

  }
  .message_bubble .content > div {
    margin:5px;
    margin-right:10px;
  }


  .right .content{
    flex-direction :row-reverse ;
    background : #dadada;
    border-radius : 50px;

  }
  .left .content{
    background : #B3E5FC;
    border-radius : 50px;
  }

  .right .timestamp {
    text-align : right;
  }
  .timestamp {

    font-size : 10px;
    color: #000;
    letter-spacing : 2px;
  }
  .content .author {
    height : 40px;
    width:40px;
    min-width:40px;
    background : #000;
    color : #fff;
    text-align : center;
    font-size : 10px;
    line-height : 40px;
    border-radius : 50px;
  }
</style>
