<template>
  <div>

<!--    https://www.youtube.com/watch?v=oCxEXfsld-o&list=PLcoYAcR89n-qTYqfWTGxXMnAvCqY3JF8w&index=7-->
    <!-- Pode-se suprimir v-bind usando somente ':' -->
<!--    <img :src="imgSrc" v-bind:alt="imgAlt"> -->

    <h1 :class="{title: true, 'title-home': isHome }">
      Curso de Vue 3
    </h1>

    <p :class="['text', {'text-home': isHome }]">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias aspernatur dolor dolores eos error et explicabo fugit hic impedit ipsa ipsum labore libero nihil optio pariatur, perspiciatis quia repellat vel?
    </p>

    <p :style="styleClass">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. A aliquam neque, non obcaecati possimus provident voluptas. Beatae cumque eius facilis labore, laudantium magnam, placeat quasi ratione reprehenderit sapiente, soluta voluptatibus.
    </p>

    <div v-for="(obj, index) in todos" v-bind:key="obj.id" class="todos-item">
      <img
          v-if="obj.imgSrc"
          v-bind:src="obj.imgSrc">
      {{index}} - {{ obj.title }}
    </div>

  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      isHome: true,
      classVar: 'title',
      styleClass: {color: 'aqua', backgroundColor: 'black', 'font-size': '20px'},
      pClass:['text', 'text-home'],
      todos: [
        {
          "userId": 1,
          "id": 1,
          "title": "delectus aut autem",
          "completed": false,
          "imgSrc": 'https://fakeimg.pl/200x200',
        },
        {
          "userId": 1,
          "id": 2,
          "title": "quis ut nam facilis et officia qui",
          "completed": false,
          "imgSrc": 'https://fakeimg.pl/200x200',
        },
        {
          "userId": 1,
          "id": 3,
          "title": "fugiat veniam minus",
          "completed": false
        },
        {
          "userId": 1,
          "id": 4,
          "title": "et porro tempora",
          "completed": true
        },
        {
          "userId": 1,
          "id": 5,
          "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
          "completed": false
        }
      ]
    }
  }
}
</script>

<style>
.title {
  font-size: 20px;
  color: blue;
}

.title-home {
  font-size: 40px;
  color: green;
}

.text {
  color: yellowgreen;
}

.text-home {
  color: blueviolet;
}

.todos-item{
  background: black;
  color: white;
  margin: 0 0 5px 0;
  padding: 3px 6px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px;
}
</style>