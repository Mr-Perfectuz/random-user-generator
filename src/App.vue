<template>
<div class="container">
    <HeaderForm title="Task Tracker"/>
    <TasksForm :tasks="tasks"/>
</div>

</template>

<script>
import HeaderForm from './components/Header.vue'
import TasksForm from './components/Tasks.vue'

export default {
  name: 'App',
  components: {
    HeaderForm,
    TasksForm,
  },
  data() {
    return {
      tasks:[],
    }
  },
  created(){
      this.tasks = [
        {
          id: 1,
          text: "Doctors Appointment",
          day:"March 1st at 2pm",
          reminder: true,

        },
        {
          id: 2,
          text: "Meeting at school",
          day:"March 13rd at 10:00am",
          reminder: true,

        },
        {
          id: 3,
          text: "Food Shopping",
          day:"March 2st at 03:00pm",
          reminder: false,

        },

      ]
  }
}
</script>

<style>

</style>
