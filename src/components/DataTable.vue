<template>
    <v-table> 
      <thead>
     
        <tr>
          <th class="text-left font-weight-black text-white bg-grey-darken-3">
            Author
          </th>
          <th class="text-left font-weight-black text-white bg-grey-darken-3">
            Title
          </th>
          <th class="text-left font-weight-black text-white bg-grey-darken-3">
            Content
          </th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="item in data"
          :key="item.title"
        >
          <td>{{ item.author}}</td>
          <td>{{ item.title}}</td>
          <td>{{ item.content}}</td>

        </tr>
      </tbody>
    </v-table>
  </template>

<script setup>
import { ref } from "vue";
function datas(author,title,content) {
  this.author = author;
  this.title = title;
  this.content = content;
}
const data = ref([]);
var postJson
var userJson

  fetch('https://jsonplaceholder.typicode.com/posts/')
  .then((response) => response.json())
  .then((json)=>{postJson=json})
  .then(fetch('https://jsonplaceholder.typicode.com/users/')
  .then((response) => response.json())
  .then((json)=>{userJson=json})
  .then( (json) => {
    if(postJson.length!=undefined){
      for(let i=0;i<postJson.length;i++){
        var uId=postJson[i].userId -1
        data.value.push(new datas(userJson[uId].name,postJson[i].title,postJson[i].body))
      }
    }
     
  }))
</script>