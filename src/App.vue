<template>
<!-- <h1>Hello World</h1> -->
 <!-- <HelloWorld :sub-title="subTitle"/> -->
 <!-- {{ subTitle }} -->
   <!-- <HelloWorld :name="name" :age="age"/> -->
   <!-- <HelloWorld :user="user"/>
   <input type="text" v-model="user.name">
   <input type="text" v-model="user.age"> -->
   <HelloWorld :user="user"/>
   <!-- <div 
   v-if="user.age > 15">
    Mon age

   </div>
   <div 
   v-else >
   Else

   </div> -->
   <input type="text" v-model="user.name" >
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue';
// import { ref } from 'vue';
// const subTitle = "lOrem ipsum dolor sit amet.";
// const subTitle = ref ("Lorem ipsum dolor sit amet.")
// const name = ref(value:"NordCoders");
// const age = ref(value: 30);
// const user = ref ( value: {
//     name: 'NordCoders',
//     age:30,
// });
// const display = () => {
// console.log(name.value, age.value);
// }
// display()
import { reactive } from 'vue';
const user = reactive ({
    name: 'NordCoders',
    age:30,
});
const display = () =>{
    console.log(user.name, user.age);
}
display()
</script>



<style scoped>


</style>
