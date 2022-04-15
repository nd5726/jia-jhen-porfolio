<template>
  <div class="home min-h-screen flex w-full flex-col justify-center py-16">
    <main class="w-full max-w-[1000px] px-[30px] sm:px-[60px] mx-auto">
      <h2 class="flex flex-col justify-start text-3xl font-bold before:content-[''] before:mb-6 before:h-[8px] before:w-[60px] before:bg-opacity-30 before:bg-black ">關於我</h2>
      <div class="w-full mt-12 flex flex-col md:flex-row">
        <div class="w-full md:w-1/2 bg-[#E5E5E5] shadow-custom p-12 flex flex-col items-center">
          <img src="../assets/photo.png" alt="Cheng Jia-Jhen" class="w-full max-w-[230px]">
          <p class="font-bold text-xl flex flex-col items-center pt-8 after:content-[''] after:mt-8 after:h-[5px] after:w-[60px] after:bg-opacity-30 after:bg-black ">Jia-Jhen Cheng</p>
          <p class="font-bold text-lg pt-12 tracking-wider">希望職位  /  前端工程師<br>工作地點  /  台中、遠端</p>
        </div>
        <div class="w-full md:w-1/2 bg-none py-16 pl-8 sm:pl-16 pr-8 sm:pr-16 lg:pr-24 ">
          <p class="font-bold text-lg leading-8 tracking-wider">嗨，您好<br>我是鄭佳真，喜歡挑戰冒險但又謹慎，個性隨和但是不隨便。</p>
          <button @click="Goto" type="button" class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] text-white rounded-full px-8 py-2.5 my-12 shadow-lg">看看我的作品</button>
          <p class="flex font-bold"><span class="w-[80px]">EMAIL.</span>nd5726@gmail.com</p>
          <p class="flex font-bold"><span class="w-[80px]">TEL. </span>0988-858853</p>
        </div>
      </div>
    </main>
  </div>
  <div class="bg-[#F3F3F3] pt-20" ref="main">
    <h2 class="flex flex-col items-center mb-16 text-3xl font-bold before:content-[''] before:mb-6 before:h-[8px] before:w-[60px] before:bg-opacity-30 before:bg-black ">前端專案</h2>
    <div class="max-w-[1000px] px-[30px] sm:px-[60px] mx-auto pb-20">
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">妥妥手做</p>
              <p class="font-light mt-1">購物網站前端 /  設計</p>
            </div>
            <p class="pl-12 pt-5 pr-6 flex flex-wrap font-bold">
              <span class="mr-2">#網站設計</span>
              <span class="mr-2">#Vue.js</span>
              <span class="mr-2">#Vue Router</span>
              <span class="mr-2">#Vue CLI</span>
              <span class="mr-2">#Tailwind CSS</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://nd5726.github.io/total/#/">瀏覽網站</a>
          </div>
        </div>
        <div class="flex-shrink-0">
          <img src="../assets/w01.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">CNC零件打樣一站式整合平台</p>
              <p class="font-light  mt-1">前端 /  設計</p>
            </div>
            <p class="pl-12 pt-5 pr-6 text-base flex flex-wrap font-bold">
              <span class="mr-2">#網站設計</span>
              <span class="mr-2">#Alpine.js</span>
              <span class="mr-2">#Tailwind CSS</span>
              <span class="mr-2">#blade</span>
            </p>
            <p class="font-light pl-12 mt-4">*因保密協議，無法提供網站連結</p>
          </div>
          <div class="flex justify-end mb-7">
            <button @click="openModal" type="button" class="relative top-0 hover:-top-1 transition-all bg-[#E5E5E5] rounded-full text-black font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg">瀏覽設計稿</button>
          </div>
        </div>
        <div class="flex-shrink-0">
          <img src="../assets/w02.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">iCAKU 愛庫家居</p>
              <p class="font-light mt-1">形象詢價網站前端 / 設計 / 規劃 </p>
            </div>
            <p class="pl-12 pr-12 pt-5 flex flex-wrap font-bold">
              <span class="mr-2">#網站規劃</span>
              <span class="mr-2">#網站部分設計</span>
              <span class="mr-2">#RWD</span>
              <span class="mr-2">#JQuery</span>
              <span class="mr-2">#Swiper</span>
              <span class="mr-2">#WOW.js</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://www.ezgoshop.com.tw/">瀏覽網站</a>
          </div>
        </div>
        <div class="flex-shrink-0">
          <img src="../assets/w03.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">大雋聯合建築師事務所</p>
              <p class="font-light mt-1">形象作品網站前端 / 規劃</p>
            </div>
            <p class="pl-12 pt-4 pr-6 flex flex-wrap font-bold">
              <span class="mr-2">#RWD</span>
              <span class="mr-2">#網站規劃</span>
              <span class="mr-2">#JQuery</span>
              <span class="mr-2">#tinyMap</span>
              <span class="mr-2">#Swiper</span>
              <span class="mr-2">#LazyLoad</span>
              <span class="mr-2">#SCSS</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://www.tec-archi.com.tw/">瀏覽網站</a>
          </div>
        </div>
        <div  class="flex-shrink-0">
          <img src="../assets/w04.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">站前國王商圈</p>
              <p class="font-light mt-1">平台網站前端</p>
            </div>
            <p class="pl-12 pt-4 pr-6 flex flex-wrap font-bold">
            <span class="mr-2">#地圖與店家對應功能</span>
              <span class="mr-2">#RWD</span>
              <span class="mr-2">#JQuery</span>
              <span class="mr-2">#Animation</span>
              <span class="mr-2">#SCSS</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://tcdaijiaking.com.tw/">瀏覽網站</a>
          </div>
        </div>
        <div  class="flex-shrink-0">
          <img src="../assets/w05.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">防災教育館·消防史料館</p>
              <p class="font-light mt-1">無障礙網站前端</p>
            </div>
            <p class="pl-12 pt-4 pr-6 flex flex-wrap font-bold">
              <span class="mr-2">#無障礙AA等級網站</span>
              <span class="mr-2">#RWD</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://dper.tncfd.gov.tw/">瀏覽網站</a>
          </div>
        </div>
        <div  class="flex-shrink-0">
          <img src="../assets/ww.png" class="w-full md:max-w-[300px]" alt="防災教育館·消防史料館">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">巨東刀具</p>
              <p class="font-light mt-1">形象網站前端 / 規劃 </p>
            </div>
            <p class="pl-12 pt-4 pr-6 flex flex-wrap font-bold">
              <span class="mr-2">#RWD</span>
              <span class="mr-2">#客製化游標設計製作</span>
              <span class="mr-2">#JQuery</span>
              <span class="mr-2">#Animation</span>
              <span class="mr-2">#SCSS</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://www.art-knife.com.tw/">瀏覽網站</a>
          </div>
        </div>
        <div  class="flex-shrink-0">
          <img src="../assets/w02.jpg" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
      <div class="bg-white shadow-card flex flex-col-reverse md:flex-row max-w-[800px] w-auto mb-12">
        <div class="flex-grow  pt-12 pr-6 flex flex-col justify-between">
          <div>
            <div class="text-xl flex flex-col pl-12 relative before:content-[''] before:mb-6 before:left-0 before:absolute before:h-full before:w-[12px] before:bg-[#5ABAFF]">
              <p class="font-bold">朝和餅舖</p>
              <p class="font-light mt-1">購物網站前端</p>
            </div>
            <p class="pl-12 pt-4 pr-6 flex flex-wrap font-bold">
              <span class="mr-2">#RWD</span>
              <span class="mr-2">#JQuery</span>
              <span class="mr-2">#Animation</span>
              <span class="mr-2">#SCSS</span>
            </p>
          </div>
          <div class="flex justify-end mb-7">
            <a class="relative top-0 hover:-top-1 transition-all bg-[#5ABAFF] hover:bg-[#0B98FF] rounded-full text-white font-bold py-2.5 px-12 mt-8 md:mt-0 shadow-lg" target="_blank" href="https://www.tsao-her.com.tw/">瀏覽網站</a>
          </div>
        </div>
        <div  class="flex-shrink-0">
          <img src="../assets/w06.png" class="w-full md:max-w-[300px]" alt="">
        </div>
      </div>
    </div>
  </div>
  <DesignComponent ref="designModal"></DesignComponent>
</template>

<style lang="scss">
  .home{
    background-image: linear-gradient(90deg, #F6F6FA 40%, #ffffff 40%);
    @media (max-width:768px) {
      background-image: linear-gradient( #F6F6FA 40%, #ffffff 40%);
    }
  }
  .shadow-custom{
    box-shadow: -10px 26px 33px -1px rgba(0, 0, 0, 0.25);
    @media (max-width:768px) {
      box-shadow: -10px 15px 15px -1px rgba(0, 0, 0, 0.25);
    }
  }
  .shadow-card{
    box-shadow: 13px 12px 31px -6px rgba(0, 0, 0, 0.25);
  }
</style>

<script>
import DesignComponent from '@/components/DesignComponent.vue'
export default {
  methods: {
    Goto () {
      const target = this.$refs.main.offsetTop
      window.scrollTo({ top: target })
    },
    openModal () {
      this.$refs.designModal.showFormModal = true
    }
  },
  components: {
    DesignComponent
  }
}
</script>
