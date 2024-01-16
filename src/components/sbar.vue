<template>
 <div class=" fixed w-screen nav-bar bg-gray-800 ">
   <button @click="toggleSidebar"  class="cursor-pointer">
   <div class="text-white float-left p-2">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
          </svg> 
     </div>
     </button>
    <div class=" text-white w-35 h-10 bg-red-500 w-9 p-2 float-right">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 9V5.25A2.25 2.25 0 0 1 10.5 3h6a2.25 2.25 0 0 1 2.25 2.25v13.5A2.25 2.25 0 0 1 16.5 21h-6a2.25 2.25 0 0 1-2.25-2.25V15M12 9l3 3m0 0-3 3m3-3H2.25" />
          </svg>
    </div>
 </div>
<div class="w-screen h-auto  flex bg-gray-200">
<div class="w-[260px] fixed top-9 h-full" v-if="showSidebar" >
 <div
      class="sidebar-header h-10 w-full p-2  bg-gray-800  font-medium items-center ">
      <span class="text-white product pl-3">PRODUCT
        <span class="text pl-24 ">QTY</span>
      </span>
    </div>
    <div
      class="bg-gray-700 p-2 text-center items-center justify-center flex h-10"
    >
      <h6
        class="Seafood font-sans flex-nowrap text-white font-semibold opacity-95"
      >
        S E A F O O D S
      </h6>
    </div>
    <div class="seafood-lists items-center flex flex-nowrap flex-row  bg-gray-800 p-5">
      <ul>
        <li
          class="seafood-items flex flex-row flex-nowrap text-white font-semibold text-md mb-2"
        >
          Salmon Grill
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-auto ml-20 float-right  "
            >2</span
          >
        </li>
        <li
          class="seafood-items text-white flex flex-nowrap font-semibold text-md  mb-2"
        >
          Miso Salmon
          <span
            class="rounded-md w-6 h-6 bg-gray-700  text-md text-center ml-auto float-right "
            >3</span
          >
        </li>
        <li class="seafood-items text-white font-semibold text-md mb-2">
          Sea Bass Grill
          <span
            class="rounded-md w-6 h-6 bg-gray-700  text-md text-center ml-auto float-right "
            >4</span
          >
        </li>
        <li class="seafood-items text-white font-semibold text-md mb-2">
          Grilled Calamari
          <span
            class="rounded-md w-6 h-6 bg-gray-700  text-md text-center ml-auto float-right"
            >1</span
          >
        </li>
      </ul>
    </div>
     <div
      class="bg-gray-700 text-center items-center justify-center flex h-10"
    >
      <h6
        class="Soup p-2 font-sans flex-nowrap text-white font-semibold opacity-95">
      S O U P S
      </h6>
     </div>
     <div class="seafood-lists items-center flex flex-nowrap bg-gray-800 p-5">
      <ul>
        <li
          class="seafood-items text-white flex flex-nowrap flex-row font-semibold text-md mb-2 "
        >
          Lobster Bisque
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-auto ml-16 float-right"
            >4</span
          >
        </li>
        <li
          class="seafood-items  text-white flex flex-nowrap font-semibold text-md  mb-2"
        >
          Tomato Soup
          <span
            class="rounded-md w-6 bg-gray-700 text-md text-center ml-auto float-right"
            >2</span>
        </li>  
      </ul>
    </div>
     <div
      class="bg-gray-700 border-none shadow-none text-center items-center justify-center flex h-10"
    >
      <h6
        class="Soup p-2  font-sans flex-nowrap text-white font-semibold opacity-95">
      S A L A D S
      </h6>
     </div>
      <div class="seafood-lists items-center flex flex-nowrap bg-gray-800 p-5">
      <ul>
        <li
          class="seafood-items text-white flex flex-nowrap flex-row font-semibold text-md mb-2"
        >
          Caesar Salad
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-20 float-right"
            >4</span
          >
        </li>
         <li
          class="seafood-items text-white flex flex-nowrap flex-row font-semibold text-md mb-2"
        >
         Spicy Carrot Salad
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-auto float-right"
            >1</span
          >
        </li>
         <li
          class="seafood-items text-white flex flex-nowrap flex-row font-semibold  text-md mb-2"
        >
         Salmon Sushi Salad
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-auto  float-right"
            >1</span
          >
        </li>
         <li
          class="seafood-items text-white flex flex-nowrap flex-row font-semibold text-md mb-2"
          >
          Quinoa Salad
          <span
            class="rounded-md w-6 h-6 bg-gray-700 text-md text-center ml-auto  float-right"
            >1</span
          >
        </li>
      </ul>
       </div>
       </div>

       <div class=" w-full justify-center items-center relative lg:ml-64 pr-5 h-full top-9 bg-gray-200 ">
       <div class="cards  grid grid-cols-1 xl:grid-cols-4 lg:grid-cols-3 md:grid-cols-2 sm:grid-cols-1 space-x-5 justify-center items-center mb-3 mx-auto ">
 <div class="card bg-white ml-5 mt-5  ">
  <div class="card-header h-16 bg-red-600 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in firstListItem"  :key="item" :list="list" ></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5  ">
  <div class="card-header h-16 bg-red-600 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in secondListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5  ">
  <div class="card-header h-16  bg-green-400 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in thirdListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5 ">
  <div class="card-header h-16 bg-green-400 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in fourthListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5  ">
  <div class="card-header h-16 bg-green-400 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in fifthListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5  ">
  <div class="card-header h-16 bg-green-400 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in sixthListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
  <div class="card bg-white mt-5 ml-5  ">
  <div class="card-header h-16 bg-green-400 ">
      <span class="header-text-left font-semibold pl-2 pt-2 text-white opacity-90">18:27 <br>
    Table:R14
    </span>
    <span class="header-text-right font-semibold pl-2 pt-2 text-white opacity-90 " >Jane S.
        <br>
        #2044
    </span>
     </div>
     <div class="card-body">
<ul>
<list-component  v-for="(list,item) in seventhListItem"  :key="item" :list="list  "></list-component>
</ul>
</div>
 </div>
       </div>
       </div>
</div>
</template>

<script>
import list from './list.vue'
import ListComponent from './ListComponent.vue'
export default{
name:"sbar" ,
components:
{
list,
ListComponent
},
data() {
     return {  
      showSidebar:true ,
      firstListItem:[
            {
                product: "Salmon Grill",
                uantity: 1,
                modifiers: ["NO SALT",] ,
                
            },
            {
                product: "Lobster bisque",
                uantity: 2,
                modifiers: ["MEDIUM",] ,
                
            },
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["ADD CHEESE",],
                 
            },
            {
                product:"Brocolli",
                uantity:1,
                modifiers:[" ",],
            }
        ] ,
       secondListItem: [
            {
                product: "Grilled Calamari",
                uantity: 1,
                modifiers: ["EXTRA SAUCE",] ,
                
            },
            {
                product: "Sea Bass Grill",
                uantity: 2,
                modifiers: ["MEDIUM",] ,
                
            },
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["REMOVE OLIVES",],
                 
            },
            {
                product:"Tomato Soup",
                uantity:1,
                modifiers:[" ",],
            }
        ],
        thirdListItem: [
            {
                product: "Sea Bass Grill",
                uantity: 1,
                modifiers: ["ADD POTATOES",] ,
                
            },
            {
                product: "Miso Salmon",
                uantity: 2,
                modifiers: ["NO SALT",] ,
                
            },
            {
                product: "Grilled Calamari",
                uantity: 1,
                modifiers: ["1.5 PORTION",],
                 
            },
            {
                product:"Brocolli",
                uantity:1,
                modifiers:["",],
            }
        ],
        fourthListItem: [
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["EXTRA CHICKEN",] ,
                
            },
            {
                product: "Quinoa Salad",
                uantity: 2,
                modifiers: ["REMOVE LETTUCE",] ,
                
            },
            {
                product: "Salmon Sushi Salad",
                uantity: 1,
                modifiers: ["ADD CHEESE",],
                 
            },
            {
                product:"Spicy Carrot Salad",
                uantity:1,
                modifiers:["",],
            }
        ],
        fifthListItem: [
            {
                product: "Sea Bass Grill",
                uantity: 1,
                modifiers: ["NO SALT",] ,
                
            },
            {
                product: "Miso Salmon",
                uantity: 2,
                modifiers: ["REMOVE HERBS",] ,
                
            },
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["ADD CHEESE",],
                 
            },
            {
                product:"Brocolli",
                uantity:1,
                modifiers:["",],
            }
        ],
        sixthListItem: [
            {
                product: "Salmon Grill",
                uantity: 1,
                modifiers: ["NO SALT",] ,
                
            },
            {
                product: "Lobster Bisque",
                uantity: 2,
                modifiers: ["MEDIUM",] ,
                
            },
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["ADD CHEESE",],
                 
            },
            {
                product:"Tomato Soup",
                uantity:1,
                modifiers:["",],
            }
        ],
        seventhListItem: [
            {
                product: "Tomato Soup",
                uantity: 1,
                modifiers: ["ADD CHEESE",] ,
                
            },
            {
                product: "Miso Salmon",
                uantity: 2,
                modifiers: ["GRILLED POTATOES",] ,
                
            },
            {
                product: "Caesar Salad",
                uantity: 1,
                modifiers: ["ADD CHEESE",],
                 
            },
            {
                product:"Brocolli",
                uantity:1,
                modifiers:["",],
            }
        ],
     }

},
methods:{
  toggleSidebar(){
    this.showSidebar=!this.showSidebar;
  }
}
}
</script>


<style>
.nav-bar{
  width:auto;
  height: 40px;
}
.card{
    height: 300px;
    
}
.header-text-left{
font-size:14px;
float: left;
}
.header-text-right{
    float: right;
    padding-right: 20px;
    font-size: 14px;
}



</style>