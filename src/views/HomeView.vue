<template>
  <main class="container font-style">

      <image-with-steps/>
      <steps-for-buying-on-a-lizing/>
      <physical-person/>
      <hr/>
      <juridica-person :list-jurisdiction-person="jurisdictionPersonList"/>
      <hr/>
      <p class="text-danger fs-5 me-md-5 pe-md-5"><i>* НАПОМЕНА: ДОКОЛКУ ПОДАТОЦИТЕ КОИ ГИ ОСТАВАТЕ ПРИ ПРЕД-ОДОБРУВАЊЕТО НЕ СЕ ТОЧНИ И ПРЕЦИЗНИ МОЖНО Е АПЛИКАЦИЈАТА ЗА ЛИЗИНГ ДА ВИ БИДЕ ОДБИЕНА ИЛИ ПРОЛОНГИРАНА ОД СТРАНА НА БАНКАТА И ПРИТОА ГО ГУБИТЕ ОСТАВЕНИОТ КАПАР.</i></p>

  </main>
</template>

<script>

import ImageWithSteps from "@/components/ImageWithSteps";
import StepsForBuyingOnALizing from "@/components/StepsForBuyingOnALizing";
import PhysicalPerson from "@/components/PhysicalPerson";
import JuridicaPerson from "@/components/JuridicaPerson";

export default {
  name: 'HomeView',
  components: {ImageWithSteps,
      StepsForBuyingOnALizing,
      PhysicalPerson,
      JuridicaPerson},

}
</script>
