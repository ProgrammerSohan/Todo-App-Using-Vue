<script setup>
/*
import { ref, computed } from "vue"
const 
 _todo_text = ref(""),    
 _todo_list = ref([]),
 _pending = computed(() => {
     return _todo_list.value.filter(item => !item.checked)
 }),
 _done*/


</script>

<template>
    <div class="todo-container w3-white w3-card-4">
        
        <div class="w3-container w3-black w3-margin-0
        w3-bottombar w3-border-blue">
        <h1>
        <i class="fa-solid fa-clipboard-list"></i>
        To-Do List
        </h1>
       </div>
       <!--user input-->
       <div class="w3-container flex-container w3-light-gray w3-padding">
        <input  class="w3-input w3-border-0" 
                type="text" 
                autofocus
               
                placeholder="Type here your to-do item...">
        <button class="w3-button w3-gray" >
            <i class="fa-solid fa-times"></i>
        </button>
        <button class="w3-button w3-blue">
            <i class="fa-solid fa-plus"></i>
        </button>
    </div>

     <!-- List of pending items -->
     <div class="w3-padding w3-blue">Pending </div>
     <div class="w3-padding">
         <label>
             <input type="checkbox" >
             <span class="w3-margin-left">
             
             </span>
         </label>
     </div>
     <div class="w3-padding" >No tasks</div>

      <!-- List of completed tasks -->
      <div class="w3-padding w3-blue">Completed </div>
      <div class="w3-padding" >
          <label>
              <input type="checkbox" >
              <span class="w3-margin-left">
               
              </span>
          </label>
      </div>
      <div class="w3-padding" >No tasks</div>
        
    </div>

</template>

<style scoped>
.todo-container {
    max-width: 100%;
    min-width: 30rem;
}

label {
    cursor: pointer;
    display: flex;
}
</style>

