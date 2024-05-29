<template>
  <!-- <div class="container"> -->

  <!-- <div class="flex gap-6 bg-gray-300 justify-around flex-col sm:flex-row pb-10 ">
      <div class="sm:w-1/3 flex flex-col w-full px-5">
    
        <img
          src="@/assets/room1.jpg"
          alt="room1"
          class="aspect-video w-full object-cover  w-64 text-justify rounded-md rounded"
        />
        <h4 class="font-bold">{{ title }}</h4>
        
        <span>Sun,5 May</span>
        <p class="pb-5">>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis,
          delectus.
        </p> -->
  <!-- <a href="">Read More</a> -->
  <!-- <div class="flex gap-6 bg-gray-300 justify-around flex-col sm:flex-row pb-10  "> -->
    <div class="sm:w-1/3 flex flex-col w-full px-5 ">
      <img src="@/assets/room1.jpg" alt="room1"
        class="aspect-video w-full object-cover  w-64 text-justify rounded-md rounded  " />
      <h4 class="font-bold">{{ title }}</h4>
      <span>{{ date }}</span>
      <!-- <span>Sun,5 May</span> -->
      <p class="pb-5">
       {{ content }}.
      </p>
  <RouterLink to="/singlepage" class="no-underline text-white font-bold px-5 py-2 bg-red-400 rounded w-fit ">Read More</RouterLink> 

    </div>
  


</template>
<script setup>
const props = defineProps({
  title: {
    default: ''
  },
  date: {
    default: ''
  },
  content: {
    default:''
  }
})
console.log(props.default)
</script>