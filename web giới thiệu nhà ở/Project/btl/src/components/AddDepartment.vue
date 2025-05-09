<template>
    <div class="container col-md-6">
      <form  @submit.prevent="AdminPage">
       
        <h1>Thêm căn hộ</h1>
        <div id="error-summary">
          <label for="title">căn hộ </label>
          <input type="text"  name="name" class="form-control" v-model="projects.name" required />

          <label for="title">Địa chỉ</label>
          <input type="text"  name="address" class="form-control" v-model="projects.address" required />

          <label for="price">Giá</label>
          <input type="text"  name="price" class="form-control"  v-model="projects.price" required />

          <label for="type">image</label>
          <input type="text"  name="image" class="form-control"  v-model="projects.image" required />

          <div class="mt-3">
        <input type="submit"  class="btn btn-primary" value="">
      </div>
        </div>
      </form>
      <router-view />
    </div>

  </template>
  <script>
  import axios from "axios";
 
  export default {
    data() {
      return {
        projects:{
        name: "",
        address: "",
        price: "",
        image:"",
        },
      };
    },
    methods:{
      AdminPage(){
        axios.post('https://657fc7106ae0629a3f53a003.mockapi.io/projects', this.projects)
        .then(response=>{
          
          this.$router.push('/admin-page');
          console.log(response.status);
        })
        .catch(error=>{
          
          console.log(error);
        })
      },
      
    }
   
  }
  </script>
<style scoped>
*{
    margin : 10px;
}
</style>