<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
      <div class="container">
        <div class="row">
          <div class="col-md-2">
            <ul class="list-group">
              <li class="list-group-item">원래대로</li>
              <li class="list-group-item" >가격순</li>
              <li class="list-group-item" >예제버튼</li>
            </ul>
          </div>
        
    <div class="col-md-10">
      <div class="row">
        <Card  v-for="(item,i) in rooms" v-bind:oneroom="item" v-bind:key="i"/>
      </div>
    </div>
  </div>
</div>
    
 
  </div>
</template>

<script>
import Card from './components/Card.vue';
import Post from './data/post.js';

export default {
  name: 'app',
  data() {
    return  {
      rooms : Post
    }
  },
 
  components: {
    Card
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
