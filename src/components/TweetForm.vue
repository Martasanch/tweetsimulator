<template>
 <div class="tweet-form container" :class=" {open: showForm}">
     <form>
         <input class="form-control" placeholder="Tu nombre"/>
         <textarea 
         class="form-control"
         rows="3"
         placeholder="Escribe tu mensaje">
         </textarea>
         <button type="button" class="btn btn-primary pl-4 pr-4">Enviar Tweet</button>
     </form>
 </div>

</template>

<script>
export default {
name: 'TweetForm',
props:{
    showForm:Boolean,
}
}
</script>


<style lang="scss" scoped>

 .tweet-form{
  margin-top: 20px;
  height: 0px;
  overflow: hidden;
 
  &.open{
      height: auto;
  }
  form{
  margin-bottom: 50px;
  input{
  margin-bottom: 10px;

  }
  button{
    width: 100%;
    margin-top: 10px;
  }
}
}



</style>

