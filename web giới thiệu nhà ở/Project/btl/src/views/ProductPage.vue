<template>
   
    <div class="container col-md-12">
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
      </div>
   
  </template>
  
  <script>
  import axios from "axios";
  export default {
      data(){
          return{
              projects:[]
          };
      },
      created(){
          axios.get("https://657fc7106ae0629a3f53a003.mockapi.io/projects").then((response)=>
          {
              this.projects=response.data;
          })
          .catch((error)=>{
          console.log(error);
      });
      },
      methods: {
    requestEmailAndConfirmOrder(book) {
      const userEmail = prompt("Nhập địa chỉ email của bạn để đặt hàng:");

      if (userEmail !== null && userEmail.trim() !== "") {
        
        if (confirm(`Bạn có chắc chắn muốn đặt hàng cuốn sách "${book.name}" không?`)) {
          alert(`Bạn đã đặt hàng thành công cuốn sách "${book.name}" và sẽ nhận được thông báo tới địa chỉ email: ${userEmail}`);
        }
      } else {
       
        alert("Đặt hàng không thành công. Vui lòng nhập địa chỉ email để đặt hàng.");
      }
    },
    }
  }
  </script>
  
  <style scoped>

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  .logo {
      width: 70px;
      height:auto;
    }
  * {
    margin: 0;
    padding: 0;
    font-family: "Poppins", sans-serif;
    box-sizing: border-box;
  }
  .menu{
    width: 100%;
    overflow: hidden;
    color:rgb(36, 75, 215);
  }
  nav {
    background: #3931d3;
    width: 100%;
    padding: 10px 10%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: relative;
  }
  
  
  nav ul {
    width: 100%;
    text-align: center;
    display:flex;
  }
  nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
  }
  nav ul li a {
    color: #fff;
    text-decoration: none;
  }
  .logo-container {
      display: flex;
      align-items: center;
      margin-left: 15px;
    }
    
    .phone-icon {
      width: 24px;
      height: 24px;
      margin-right: 5px;
    }
    
    .phone-number {
      color: #fff;
      font-weight: bold;
    }
    ul {
    list-style: none;
    display: flex;
    padding: 0;
    margin-left: 50px;
  }
  ul li {
    display: inline-block;
    margin-right: 50px;
    width: 50%;
    margin-bottom: 50px; /* Khoảng cách giữa các thẻ li */
  }
  .table {
    Width: 100%;
    table-layout: fixed;
    display: flex;
    align-items: center;
    justify-content: center;
    border-spacing: 10px;
  }
  .table {
    display: grid;
    place-items: center;
    margin : 30px auto;
  
  }
   td {
    padding: 8px;
    border: 1px solid #b74141;
  }
  </style>