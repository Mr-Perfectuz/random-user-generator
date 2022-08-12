<template>
    <header>
        <h1>{{title}}</h1>
        <ButtonForm text = "Add Task" color="lightgreen"/>
    </header>
</template>

<script>
import ButtonForm from './Button.vue'

export default {
    name: 'HeaderForm',
    props: {
        title: String
    },

    components: {
        ButtonForm
    }
}
 </script>

 <style scoped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
 </style>