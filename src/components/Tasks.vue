<template>

    <div>
        <div :key="task.id" v-for = "task in tasks">
        <h3>{{ tasks.text }}</h3>
        </div>
    </div>

</template>

<script>
export default {
    name: "TasksForm",
    proops:{
        tasks: Array,
    }
}
</script>