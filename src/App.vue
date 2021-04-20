<template>
  <div id="app">
   <div v-for="profile in employees" :key="profile.id">
     <profile-card :profile="profile" />
   </div>
  </div>
</template>

<script>
import ProfileCard from './components/ProfileCard.vue'

export default {
  name: 'App',
  components: {
    ProfileCard,
  },
  data() {
    return {
      employees: [
        {
          id: 1,
          firstName: 'Lael',
          lastName: 'Uberuaga-Rodgers',
          email: 'lael@example.com',
          phone: '(208)921-0001',
          photo: 'https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/full_width/public/thumbnails/image/placeholder-profile_1.png'
        },
        {
          id: 2,
          firstName: 'Matthew',
          lastName: 'Chertudi',
          email: 'matthew@example.com',
          phone: '(208)921-0002',
          photo: 'https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/full_width/public/thumbnails/image/placeholder-profile_1.png'
        },
        {
          id: 3,
          firstName: 'Nabil',
          lastName: 'Rahman',
          email: 'nabil@example.com',
          phone: '(208)921-0003',
          photo: 'https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/full_width/public/thumbnails/image/placeholder-profile_1.png'
        },
        { 
          id: 4,
          firstName: 'Ryan',
          lastName: 'Woodings',
          email: 'ryan@example.com',
          phone: '(208)921-0004',
          photo: 'https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/full_width/public/thumbnails/image/placeholder-profile_1.png'
        },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
