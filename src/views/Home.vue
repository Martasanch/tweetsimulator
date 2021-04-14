<template>

<Menu :openCloseForm="openCloseForm" :showForm="showForm"/>
<TweetForm :showForm="showForm"/>

</template>

<script>
import Menu from "@/components/Menu"
import TweetForm from "@/components/TweetForm"
import useFormTweet from "@/hooks/useFormTweet"
export default {
  name: 'Home',
  components: {
    Menu,
    TweetForm
 
  },
  setup(){
    return{
      ...useFormTweet() //con ... obtengo solo el contenido
    }
  }
}
</script>
