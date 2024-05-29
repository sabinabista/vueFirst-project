<script setup>
import BlogItem from './blog/BlogItem.vue';
import {ref} from 'vue'


// import WelcomeItem from './WelcomeItem.vue'
// import DocumentationIcon from './icons/IconDocumentation.vue'
// import ToolingIcon from './icons/IconTooling.vue'
// import EcosystemIcon from './icons/IconEcosystem.vue'
// import CommunityIcon from './icons/IconCommunity.vue'
// import SupportIcon from './icons/IconSupport.vue'

const data = [
  {
    title:'Blog A',
    date:'may5,2022',
    content:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis delectus',
        

  },
  {
    title:'Blog B',
    date:'may4,2022',
    content:' Room have twobunk beds.Four people per room.learn about differnt hostel room type and expect in your room',

  },
  {
    title:'Blog C',
    date:'may6,2022',
    content:' most hostel feature shared bathroom ,a communal kitchen and a common area where you can work,hang out and meet other travelers',
  }
]

const showTitle = ref(true


)

</script>

<template>

<section>
      <!-- <img
         src="@/assets/Room.jpg" 
        alt="Room"
        height="600px"
        width="100%"
      />
      <!<div class="absolute"> -->
        <!-- <h1>Girls Hostel</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non porro a fuga mollitia cum doloribus eligendi, totam ipsam. Est ullam quas sunt animi, vel consequatur obcaecati odit. Nostrum, pariatur corporis. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque iusto tenetur explicabo consectetur voluptates ex cupiditate possimus quaerat cumque aperiam quidem nisi, enim a accusamus, expedita sunt deserunt quia ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab dolor aliquid at velit totam temporibus quidem atque ullam quibusdam quos facilis tenetur enim suscipit cumque beatae ipsum, perspiciatis magnam nesciunt!</p> -->

       

      <!-- </div> -->
      <!-- <div class="absolute top-20 flex flex-col items-center  p-4">
        <h1 class="text-white text-3xl font-bold ">Girls Hostel</h1>
        <p class="text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non porro a fuga mollitia cum doloribus eligendi, totam ipsam. Est ullam quas sunt animi, vel consequatur obcaecati odit. Nostrum, pariatur corporis. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque iusto tenetur explicabo consectetur voluptates ex cupiditate possimus quaerat cumque aperiam quidem nisi, enim a accusamus, expedita sunt deserunt quia ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab dolor aliquid at velit totam temporibus quidem atque ullam quibusdam quos facilis tenetur enim suscipit cumque beatae ipsum, perspiciatis magnam nesciunt!</p>

    </div>  -->
    <img
       class="h-screen"
        src="@/assets/Room.jpg"
        alt="Room"
        style="object-fit: cover;"
        width="100%"
        
      />
      <div class="absolute top-20 flex flex-col items-center  p-4 top-52">
        <h1 class="text-white text-3xl font-bold " v-if="showTitle">Girls Hostel</h1>
        <p class="text-white pt-7 drop-shadow-xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non porro a fuga mollitia cum doloribus eligendi, totam ipsam. Est ullam quas sunt animi, vel consequatur obcaecati odit. Nostrum, pariatur corporis. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque iusto tenetur explicabo consectetur voluptates ex cupiditate possimus quaerat cumque aperiam quidem nisi, enim a accusamus, expedita sunt deserunt quia ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab dolor aliquid at velit totam temporibus quidem atque ullam quibusdam quos facilis tenetur enim suscipit cumque beatae ipsum, perspiciatis magnam nesciunt!</p>

    </div>

    </section>
    <section class="flex flex-col items-center py-10 ">
      <h1>OUR SERVICES</h1>
      <p > Girls hostel in Nepal based on cheap price, located and facilities for girls with top rating view.</p>
    </section>
    

    <!-- <div class="cards">  -->
      <div class="flex gap-6 bg-gray-300 justify-around flex-col sm:flex-row pb-10 ">
        
      <BlogItem v-for="b in data" :key="b.index" :title="b.title" :date="b.date" :content="b.content"></BlogItem>
      
    <!-- <div class="flex gap-6 bg-gray-300 justify-around flex-col sm:flex-row pb-10 "></div>
      <div class="sm:w-1/3 flex flex-col w-full px-5"> -->

      
    </div> 
</template>

