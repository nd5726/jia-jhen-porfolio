<template>
  <div id="designModal" aria-hidden="true" v-show="showFormModal" class="flex fixed top-0 right-0 left-0 pt-[40px] pb-[40px] z-50 justify-center items-center  h-screen  bg-black bg-opacity-50">
    <div  @click="showFormModal=!showFormModal"  class="flex fixed right-0 left-0 h-screen  bg-black bg-opacity-50"></div>
    <div class="relative w-11/12 sm:w-2/3 rounded-lg shadow bg-white h-[calc(100vh-80px)]">
      <div class="flex justify-between items-start px-4 py-2 rounded-t">
          <h3 class="text-lg font-semibold lg:text-2xl text-white">{{ title }}</h3>
          <button type="button" @click="showFormModal= false" class="text-gray-400 bg-transparentrounded-lg text-sm p-1.5 ml-auto inline-flex items-center hover:bg-gray-600 hover:text-white" data-modal-toggle="defaultModal">
          <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
          </button>
      </div>
      <div class="p-6 flex flex-col overflow-y-auto  h-[calc(100%-65px)]">
        <img src="../assets/dashboard.png" class="w-full shadow-xl mb-8" alt="">
        <img src="../assets/part-editPage.jpg" class="w-full shadow-xl mb-8" alt="">
        <img src="../assets/quote-request.jpg" class="w-full shadow-xl mb-8" alt="">
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {

      showFormModal: false
    }
  },
  methods: {
  }
}
</script>
