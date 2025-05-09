<template>
    <div class="container">
    <div class="container col-md-10" >
        <table class="table">
          <thead>
            <th>STT</th>
            <th>Tên</th>
            <th>Địa chỉ</th>
            <th>Gía</th>
            <th>Hình ảnh</th>
          </thead>
          <tbody>
            <tr v-for="(value, index) in projects" :key="index">
              <td>{{ index + 1 }}</td>
              <td>{{ value.name }}</td>
              <td>{{ value.address }}</td>
              <td>{{ value.price }}</td>
              <td>
              <img :src="value.image" alt="Hình ảnh " style="max-width: 100px; max-height: 100px;" />
            </td>
            <td>
              <button class="btn btn-primary" @click="requestEmailAndConfirmOrder(value)">Đặt Hàng</button>
            </td>
            </tr>
          </tbody>
        </table>
      <button @click="them" class="btn btn-primary">Thêm căn hộ</button>
    </div>
    </div>
  </template>
  
  <script>
  import axios from 'axios';

  export default {
    data() {
      return {
        projects: [],
      };
    },
    mounted() {
      this.fetchProjects();
    },
    methods: {
      fetchProjects() {
        axios
          .get("https://657fc7106ae0629a3f53a003.mockapi.io/projects")
          .then((response) => {
            this.projects = response.data;
          })
          .catch((error) => {
            console.error("Error fetching Projects:", error);
          });
      },
      them() {
        this.$router.push('/add-pet');
      },
      
    
  },
    };
 
  </script>
  
  <style>
  .button-custom a {
    text-decoration: none;
    color:white;
    background-color: darkorange;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
  
  }
  .button-custom:hover {
    background-color: darkorange; 
    color: white; 
  }
  .container {
  align-items: center;
}
  </style>