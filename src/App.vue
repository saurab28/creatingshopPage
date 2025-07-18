<script setup>
import MyModal from './components/MyModal.vue';
// import {reactive, ref, computed} from 'vue';
//   // 
//   // let state = reactive({count : 0}) ;
//   const a = 0 ;

//   const count = ref(a) ;
//   const state = reactive({
//     sum : count
//   })
//   // state.sum = count ;
//   // count.value = 2 ;
//   const author = reactive({
//   add: 1,
//   books: [
//     'Vue 2 - Advanced Guide',
//     'Vue 3 - Basic Guide',
//     'Vue 4 - The Mystery'
//   ]
// })

// const publishedBooksMessage = computed((previous) => {
//   // console.log(author);
//   if (count.value>3){
//     return count.value
//   }
//   console.log(previous)
//   return previous ;
// })

// const increment = () => {
//   count.value++

// }

// const publishedBooksMessag = () => {
//   return count.value ;
// }
// import {ref} from 'vue' 
// import {useCounter} from './composables/counter';
// const {count : countCompasable, increment, decrement, doubleCount} = useCounter() ;
// const count = ref(0) ;
// function cardClicked() {
//   console.log('Parent Card Clicked');
// }
// function buttonClicked() {
//   console.log('Child Button Clicked');
// }
// import { ref } from 'vue';
// const open = ref(false);

// function openModal() {
//   open.value = true ;
// }

// function closeModal(){
//   open.value = false ;

// }

// function openModal2() {
//   console.log('Modal opened!');
// }

// const message = ref('')

// function sendMessage() {
//   console.log('Message sent:', message.value)
//   message.value = ''
// }

// const text = ref('')
// const firstName = ref('')
// const secondName = ref('')
// const enterEmail = ref('')
// const showMessage = () => {
//   console.log("Triggered")
// }


// function clearInput() {
//   text.value = ''
// }
</script>

<template>
   <!-- <p>{{count}}</p> -->
  <!-- <p :[argument]="rawHtml">Hey </p> -->
    <!-- <p>{{ sum }}</p>  -->
   <!-- <p>{{ countCompasable }}</p>
  <span>{{ doubleCount }}</span>
  <button @click="increment">Increase</button>
  <button @click="decrement">Decrease</button> -->
  <!-- <div @click="cardClicked" class="p-6 bg-blue-100 rounded">
    Card Component (Clicking here triggers parent)

    <button @click.stop="buttonClicked" class="mt-4 bg-green-300 px-4 py-2">
      Child Button
    </button>
  </div>

   <button @click="openModal">Open Modal</button>
    <div v-if="open" class="fixed inset-0 bg-gray-500 bg-opacity-20 flex justify-center items-center">
      <div @click.self="closeModal" class="bg-white p-6 rounded shadow-lg">
        <h2 class="text-lg font-bold">Modal Content</h2>
        <p>This is modal content. Clicking here should NOT close the modal.</p>
      </div>
    </div>

    <button @click.once="openModal2">Open Modal</button> -->
  

  <!-- keyboard event  modifiers -->
  <!--
   <input v-model="message" @keyup.enter="sendMessage" placeholder="Type and press Enter" class="border px-2 py-1" />
   <input @keydown.alt.esc="clearInput" v-model="text" class="border px-2 py-1" /> -->

   <!-- const firstName = ref() -->
    <div class="outer">
      <h3>Vue Teleport Example</h3>
      <!-- <p>hjghjghjg jhkjhkjh kjhkh kjhkjhjh kjhkjhkj kjhkjkjkjkjhkkk kjkjkjkj</p> -->
      <div>
        <MyModal />
      </div>
    </div>

   

</template>

<style scoped>
.red{
  color:red;
}
.outer{
  height:60px;
  overflow: hidden;
}

</style>


