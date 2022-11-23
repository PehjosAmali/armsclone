<template>
    <DirectoryHead/>
   <FilterSearchVue/>
   <StaffCard
   email="pehjos4@gmail.com"
   position="Jnr Associate"
   location="service center"
   phone="0201770386"
jobtype="employee"
name="Pehjos"
image="http://t3.gstatic.com/licensed-image?q=tbn:ANd9GcRJTKwRjpdsxNzNo-SM3BIBtkaCy5reGHB5O1Mcix1dtFeg4unasByxiaMGrZad1rUAjrBALAzSfE--zI0"
  
   />
    <p v-if="error">Something went wrong...</p>
    <p v-if="loading">Loading...</p>
    <p v-else v-for="character in result.characters.results" :key="character.id">
      {{ character.name }}
    </p>
    <div>hello staff</div>
  </template>
<script>
import gql from 'graphql-tag'
import { useQuery } from '@vue/apollo-composable'
import DirectoryHead from './Directory.vue'
import FilterSearchVue from './FilterSearch.vue'
import StaffCard from './StaffCard.vue'
const CHARACTERS_QUERY = gql`
  query Characters {
    characters {
      results {
        id
        name
        image
      }
    }
  }
`
export default {
name:"StaffDir"  , 
components:{
DirectoryHead,
FilterSearchVue,
StaffCard
} ,
setup () {
    const { result, loading, error } = useQuery(CHARACTERS_QUERY);
    return {
      result,
      loading, 
      error
    }
  }
}
</script>
<style scoped>
    

</style>