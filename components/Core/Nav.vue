<template>
  <div>
    <div class="flex flex-row p-4 sticky">
      <div class="flex flex-row w-1/5 ">
        <img class="w-20 " src="@/static/Picture2.png" alt="">
        <div class="flex flex-col justify-end ">
          <div class="text-4xl text-purple-700 ">
            ระบบฐานข้อมูลบุคลากร
          </div>
          <div class="text-lg text-purple-700 ">
            เพื่อสนับสนุนการวางแผนพัฒนาบุคลากร
          </div>
          <div class="text-lg text-yellow-500 ">
            คณะเทคโนโลยีสารสนเทศและการสื่อสาร มหาวิทยาลัยพะเยา
          </div>
        </div>
      </div>
      <div class="flex flex-col w-1/2">
        <div class="flex flex-row text-right text-lg justify-end">
          <div class="mr-2">
            ผู้ใช้งาน : 
          </div>
          <div>
            xxxxxxxx xxxxxxxx
          </div>
        </div>
        <div>
          <v-app-bar class="deep-purple lighten-1 ">
            <h2 class="text-2xl text-white">Course</h2> 
            <v-spacer></v-spacer>
            <v-btn v-if="token == null" @click="$router.push('/auth/login')" outlined dark>login</v-btn>
            <v-btn v-else @click="logout()" outlined dark>Logout</v-btn>
          </v-app-bar> 
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>