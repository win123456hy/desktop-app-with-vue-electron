<template>
  <div class="about">
    <button @click="showWindowAdd">Add</button>
  </div>
</template>

<script>
  import {ipcRenderer} from "electron"

  export default {
    name: 'about',

    data(){
      return {

      }
    },

    methods: {
      showWindowAdd(){
        ipcRenderer.send('openAddWindow')
      }
    }
  }
</script>
