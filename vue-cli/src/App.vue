<template>
  <div>
    <!-- <app-header v-bind:프롭스 속성 이름="상위 컴포넌트의 데이터 이름"></app-header> -->
    <app-header v-bind:propsdata="str"></app-header>
  </div>
</template>

<script>
//컴포넌트 폴더에 있는 앱해더 임포트 하기
import AppHeader from './components/AppHeader.vue';
export default {
  data: function(){
    return {
      str: 'Header'
    }
  },
  components:{
    'app-header' : AppHeader
  }
}
</script>
<style>

</style>