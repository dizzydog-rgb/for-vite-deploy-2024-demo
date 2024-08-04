<script setup>
// import { ref } from 'vue'

// const num = ref(2)
// function clickMe() {
//   num.value += 15
// }

// const text = ref('這是一段文字')
// const city = ref('台北市')
// const isChecked = ref(true)
// const arrayCheckbox = ref([])
// const radioValue = ref('男')

// const num = ref(0)
// const htmlTemplate = `<h1>這是一個HTML片段</h1>`

// setInterval(() => {
//   num.value++
// }, 500)

// const imgUrl = ref(
//   'https://images.unsplash.com/photo-1722218530021-aa1dfba50fa5?q=80&w=400&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
// )
// const isChecked = ref(false)

// v-on
// const handleClick = () => {
//   console.log('我被觸發了')
// }
// const submitForm = () => {
//   console.log('表單觸發了')
// }
// const text = ref('一段文字')

// v-for -> 搭配陣列
// const array = ref([
//   {
//     id: '1',
//     name: '小明',
//     age: 18
//   },
//   {
//     id: '2',
//     name: '小美',
//     age: 16
//   },
//   {
//     id: '3',
//     name: '阿姨',
//     age: 20
//   }
// ])

// v-if, v-else, v-show
// const isChecked = ref(false)

import VueComponent from './components/VueComponent.vue'
</script>

<template>
  <!-- <h2>{{ text }}</h2>
  <input type="text" v-model="text" /> -->

  <!-- 表單 -->
  <!-- {{ city }}
  <select name="" id="" v-model="city">
    <option value="台北市">台北市</option>
    <option value="台中市">台中市</option>
    <option value="高雄市">高雄市</option>
  </select> -->

  <!-- checkbox 1. true false 2. value -->
  <!-- {{ isChecked }}
  <input type="checkbox" v-model="isChecked" />

  <div>
    {{ arrayCheckbox }}
    <input type="checkbox" v-model="arrayCheckbox" value="阿吉" />
    <input type="checkbox" v-model="arrayCheckbox" value="小明" />
    <input type="checkbox" v-model="arrayCheckbox" value="杰倫" />
  </div> -->

  <!-- radio -->
  <!-- <div>
    {{ radioValue }}
    <input type="radio" v-model="radioValue" value="男" />
    <input type="radio" v-model="radioValue" value="女" />
  </div> -->

  <!-- <button type="button" v-on:click="clickMe">點我</button> -->

  <!-- <div>
    <h1>這個數值目前是{{ num }}</h1>
    <h1 v-text="num"></h1>

    {{ htmlTemplate }}
    <div v-text="htmlTemplate"></div>
    <div v-html="htmlTemplate"></div>
  </div> -->
  <!-- <div>
    <img v-bind:src="imgUrl" />
    <h2>可以套用在任何的屬性上</h2>
    {{ isChecked }}
    <input type="checkbox" v-model="isChecked" />
    <input type="text" v-bind:disabled="isChecked" />
    <h2>可以套用在行內樣式上</h2>
    <div class="box" v-bind:style="{ transform: isChecked ? 'rotate(45deg)' : null }"></div>
    <div class="box" v-bind:style="{ backgroundColor: isChecked ? 'purple' : 'blue' }"></div>
  </div>

  <h2>class</h2>
  需要套用的class name: 變數 -->
  <!-- <div class="box" v-bind:class="{ rotate: isChecked }"></div>  -->

  <!-- <div>
    <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
    <form action="" @submit.prevent="submitForm">
      <button type="button" v-on:click="handleClick">點我</button> -->
  <!-- button的預設type是submit -->
  <!-- <button type="submit">點我</button>
    </form>
  </div>

  <h2>事件修飾符</h2>
  <a href="#" @click.prevent="handleClick">點我</a>

  <h2>按鍵修飾符</h2>
  <input type="text" v-on:keydown.enter="handleClick" v-model="text" /> -->

  <!-- <div>
    <div>
      姓名:{{ array[0].name }} 年齡:{{ array[0].age }}
      <hr />
    </div> -->

  <!-- 一定要加上v-bind:key="item.id" -->
  <!-- v-for 以及 v-if 不能寫在同一層 -->
  <!-- <div v-for="(item, key) in array" v-bind:key="item.id">
      索引:{{ key }}姓名:{{ item.name }} 年齡:{{ item.age }}
      <div v-if="item.age > 18">大於18歲</div>
      <div v-else>小於18歲</div>
    </div>
  </div>

  <hr />
  <input type="checkbox" v-model="isChecked" /> {{ isChecked }}

  <h1 v-if="isChecked">當 isChecked == true 會顯示這行</h1>
  <h1 v-else>目前的 isChecked 為 false</h1> -->

  <!-- v-if是直接註解調元素，v-show是display: none -->
  <!-- <h1 v-show="isChecked">當 isChecked == true 會顯示這行</h1> -->

  <h1>目前是 APP.vue</h1>
  <VueComponent></VueComponent>
</template>

<style>
/* .box {
  height: 100px;
  width: 100px;
  background-color: red;
  transition: 0.5s all;
}

.rotate {
  transform: rotate(75deg);
} */
</style>
