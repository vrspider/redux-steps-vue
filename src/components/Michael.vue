<template>
  <div>
    <ol>
      <!-- Create an instance of the todo-item component -->
      <todo-item
        v-for="item in groceryList"
        v-bind:todo="item"
        v-bind:key="item.id">
      </todo-item>
    </ol>
  </div>
</template>

<script>
export default {
  name: 'Michael',
  data () {
    return {
      msg: 'Welcome to Micahel\'s first App',
      groceryList: [
        { id: 0, text: 'Vegetables' },
        { id: 1, text: 'Cheese' },
        { id: 2, text: 'Whatever else humans are supposed to eat' }
      ]
    }
  }
}

</script>

<style>

</style>
