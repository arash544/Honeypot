<template>
<section class="main-wrapper">
  <Advertising/>
  <Imageillustration/>
  <Signuptext/>
  <Techimage/>
  <Description/>
  <Locationtext/>
  <Topjobtext/>
  <Employee/>
  <Imagecareer/>
  <Descriptiontext/>
  <Statistictext/>
</section>
</template>

<script>
import Advertising from '@/components/Advertising'
import Test from '@/components/Test'
import Imageillustration from '@/components/illustration/Imageillustration'
import Signuptext from '@/components/Signup/Signuptext'
import Techimage from '@/components/tech/Techimage'
import Description from '@/components/text-description/Description'
import Locationtext from '@/components/location/Locationtext'
import Topjobtext from '@/components/Topjobtext'
import Employee from '@/components/Employee'
import Imagecareer from '@/components/free-career/Imagecareer'
import Descriptiontext from '@/components/text-description-second/Descriptiontext'
import Statistictext from '@/components/statistic/Statistictext'

export default {
components:{
  Advertising,
  Imageillustration,
  Signuptext,
  Techimage,
  Description,
  Locationtext,
  Topjobtext,
  Employee,
  Imagecareer,
  Descriptiontext,
  Statistictext,
  
  Test
}
}
</script>

<style lang="scss" scoped>
.main-wrapper{
  width: 100%;
  display:flex;
  flex-wrap:wrap ;
    @media only screen and (max-width: 768px) {
    width: 100%;
    display:flex;
    flex-wrap:wrap ;
  }
}
</style>