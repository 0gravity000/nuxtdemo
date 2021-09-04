<template>
  <div>
    <h3>v-for</h3>
    <ol>
      <li v-for="todo in todos" :key="todo.text">
        {{ todo.text }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  layout: 'LayoutSample',
  data () {
    return {
      todos: [
        { text: 'Learn JavaScript' },
        { text: 'Learn Vue' },
        { text: 'Build something awesome' }
      ]
    }
  }
}
</script>
