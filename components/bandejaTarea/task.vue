<template>
  <div class="md:flex p-6 lg:p-14 md:p-14 gap-4 md:justify-items-center">
    <!-- <h2 class="text-2xl md:text-4xl font-bold dark:text-white">Panel de tareas</h2> -->
    <h2 class="text-2xl md:text-4xl font-bold dark:text-white">Tareas asignadas a: Ivan Mendoza</h2>
    <!-- <button type="button" class="text-white bg-purple-700 hover:bg-purple-800 focus:ring-4 focus:ring-purple-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-purple-600 dark:hover:bg-purple-700 focus:outline-none dark:focus:ring-purple-800">Agregar nueva</button> -->
    </div>
  <div class="flex justify-center">   
    <div class="grid grid-cols-1 min-h-screen md:flex md:overflow-x-scroll">
      <div
        v-for="column in columns"
        :key="column.title"
        :class="['bg-gray-50 rounded-lg px-3 py-3 column-width mr-3 border-t-6', column.color]"
      >
        <p class="text-gray-700 font-semibold font-sans tracking-wide text-sm">{{ column.title }}</p>
        <draggable
          :list="column.tasks"
          :animation="200"
          :empty-insert-threshold="200"
          ghost-class="ghost-card"
          group="tasks"
          item-key="id"
        >
          <template #item="{ element }"> 
            <task-card
              :task="element"
              class="mt-3 cursor-move"
            ></task-card>
          </template>
        </draggable>
      </div>
    </div>
  </div>
</template>

<script>
import draggable from 'vuedraggable';
import TaskCard from "./taskcard.vue";

export default {
  components: {
    TaskCard,
    draggable
  },
  data() {
    return {
      columns: [
        // {
        //   title: "Por asignar",
        //   color: "border-blue-500",
        //   tasks: [
        //     {
        //       id: 1,
        //       title: "Tarea 1",
        //       date: "13/03/2025",
        //       avatar: "https://dummyimage.com/200x200/000000/fff",
        //       name: "Ivan Mendoza"              
        //     },
        //     {
        //       id: 5,
        //       title: "Tarea 5",
        //       date: "13/03/2025",
        //       avatar: "https://dummyimage.com/200x200/000000/fff",
        //       name:"Ivan Mendoza"
              
        //     },
        //     {
        //       id: 2,
        //       title: "Tarea 2",
        //       avatar: "https://dummyimage.com/200x200/000000/fff",
        //       date: "13/03/2025",
        //       name:"Ivan Mendoza"
        //     },
        //   ]
        // },
        {
          title: "En progreso",  
          color: "border-yellow-300",        
          tasks: [
            {
              id: 3,
              title: "Subir cambios",
              date: "13/03/2025",
              avatar: "https://dummyimage.com/200x200/000000/fff",
              name:"Ivan Mendoza"
            },
            {
              id: 1,
              title: "Tarea 1",
              date: "13/03/2025",
              avatar: "https://dummyimage.com/200x200/000000/fff",
              name: "Ivan Mendoza"              
            },
            {
              id: 5,
              title: "Tarea 5",
              date: "13/03/2025",
              avatar: "https://dummyimage.com/200x200/000000/fff",
              name:"Ivan Mendoza"
              
            },
            {
              id: 2,
              title: "Tarea 2",
              avatar: "https://dummyimage.com/200x200/000000/fff",
              date: "13/03/2025",
              name:"Ivan Mendoza"
            },
          ]
        },
        {
          title: "Revisando",
          color: "border-orange-400",
          tasks: []
        },
        {
          title: "Finalizado",
          color: "border-green-500",
          tasks: [
            {
              id: 4,
              title: "Modificar estilos ",
              avatar: "https://dummyimage.com/200x200/000000/fff",
              date: "13/03/2025",
              name:"Ivan Mendoza"
            },
          ]
        }
      ]
    };
  }
}
</script>

<style scoped>
.column-width {
  min-width: 320px;
  width: 320px;
}
.ghost-card {
  opacity: 0.5;
  background: #F7FAFC;
  border: 1px solid #4299e1;
}
</style>