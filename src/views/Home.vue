<template>
  <div class="home">
    <h1>Home</h1>
    <CustomText class="a1" tag="p"> Merhaba Dunya </CustomText>
    <CustomText class="a2" tag="p" size="small"> Merhaba Dunya </CustomText>
    <CustomText class="a3" tag="p" size="xsmall"> Merhaba Dunya </CustomText>
    <CustomText tag="p" size="xxsmall"> Merhaba Dunya </CustomText>
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: 'Home',
  components: {
    CustomText
  }
}
</script>
<style scoped>
.a1{
  color: rgba(var(--ba8),.5);
}
.a2{
  color: rgb(var(--b3f));
}
.a3{
  color: rgb(var(--ba8));
}
</style>
