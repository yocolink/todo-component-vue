<template>
  <div id="todo-list">
    <input v-model="todoText" placeholder="Input TODO"/>
    <button @click="add()">Add</button>
    <button @click="removeAll()">Delete all</button>

    <div v-for="(item, index) in items" :key="index">
      <span @click="done=!done">{{index}} - {{item.text}}</span>
      <button @click="remove(index)">Delete</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'todo',
  data () {
    return {
      items: [],
      todoText: ''
    }
  },
  methods: {
    add () {
      this.items.push({text: this.todoText})
      this.todoText = ''
    },
    remove (index) {
      this.items.splice(index, 1)
    },
    removeAll () {
      this.items = []
    }
  }
}
</script>

<style>

</style>
