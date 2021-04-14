<template>
 <nav class="navbar navbar-dark bg-dark">
     <div class="container">
         <span class="navbar-brand">
             Simulador de Tweets
         </span>
         <button
         class="btn btn-success pl-4 pr-4"
         :class="{ 'btn-success': !showForm, 'btn-danger': showForm, }"
         @click="openCloseForm">{{ !showForm? "Nuevo Tweet" : "Cerrar Tweet"}}</button>
     </div>
 </nav>

</template>

<script>
export default {
name: 'Menu',
props:{
    showForm: Boolean,
    openCloseForm: Function,
}
}
</script>

<style>

</style>