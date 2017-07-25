<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>

    <router-link to="/log">Go to Foo</router-link>

      <section id='foot_guide'>
          <section @click = "gotoAddress({path: '/log'})" class="guide_item0">
              <svg class="icon_style">
                  <use></use>
              </svg>
              <span>页面1</span>
          </section>

          <section @click = "" class="guide_item1">
              <svg class="icon_style">
                  <use></use>
              </svg>
              <span>页面2</span>
          </section>

          <section @click = "" class="guide_item2">
              <svg class="icon_style">
                  <use></use>
              </svg>
              <span>页面3</span>
          </section>

          <section @click = "" class="guide_item3">
              <svg class="icon_style">
                  <use></use>
              </svg>
              <span>页面4</span>
          </section>

      </section>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

#foot_guide{
    position: fixed;
    display: flex;
    background-color: #fff;
    left:0;
    right:0;
    bottom: 0;
    height: 50px;
}

.guide_item0{
    height: 50px;
    flex: 1;
    display: flex;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #0f0;
}
.guide_item1{
    height: 50px;
    flex: 1;
    display: flex;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #ff0;
}
.guide_item2{
    height: 50px;
    flex: 1;
    display: flex;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #00f;
}
.guide_item3{
    height: 50px;
    flex: 1;
    display: flex;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #f0f;
}


</style>
