<template xmlns:v-bind='http://www.w3.org/1999/xhtml' xmlns:v-on="http://www.w3.org/1999/xhtml">
    <div class='log'>
        <h1>{{log}}</h1>
        <h2>{{msg}}</h2>
        <span v-bind:title='message'>
            鼠标悬停
        </span>
        <p v-if='seen'>你看到我了</p>
        <ol>
            <li v-for='todo in todos'>
                {{todo.text}}
            </li>
        </ol>
        <p>{{input}}</p>
        <button v-on:click="reverseInput">反转</button>
    </div>
</template>

<script>
    export default {
      name: 'log',
      data () {
        return {
          log: 'hahahaha',
          msg: 'hello vue',
          message: '加载中',
          seen: true,
          todos: [
            {text: 'haha'},
            {text: 'heihei'},
            {text: 'hehehe'}
          ],
          input: 'hello'
        }
      },
      methods: {
        reverseInput: function () {
          console.log('hello')
          this.input = this.input.split('').reverse().join('')
        }
      }
    }
</script>
