<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green"/>
<!--    <AppButton text="Update Task" color="blue"/>-->
<!--    <AppButton text="Delete Task" color="red"/>-->
  </header>
</template>

<script>
import Button from './Button.vue'
export default {
  name: 'Header',
  props: {
    title: String,
  },
  components: {
    Button

  }

  // props: {
  //   title: {
  //     type : String,
  //     default: 'Hello World',
  //   }
  // }

}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-content: center;
  margin-bottom: 20px;

}
</style>