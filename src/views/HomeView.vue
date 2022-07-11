<template>
  <main class="container font-style">
    <div>
      <image-with-steps/>
      <steps-for-buying-on-a-lizing/>
      <physical-person/>
      <hr/>
      <juridica-person/>
      <hr/>
      <p class="text-danger fs-5 me-md-5 pe-md-5"><i>* НАПОМЕНА: ДОКОЛКУ ПОДАТОЦИТЕ КОИ ГИ ОСТАВАТЕ ПРИ ПРЕД-ОДОБРУВАЊЕТО НЕ СЕ ТОЧНИ И ПРЕЦИЗНИ МОЖНО Е АПЛИКАЦИЈАТА ЗА ЛИЗИНГ ДА ВИ БИДЕ ОДБИЕНА ИЛИ ПРОЛОНГИРАНА ОД СТРАНА НА БАНКАТА И ПРИТОА ГО ГУБИТЕ ОСТАВЕНИОТ КАПАР.</i></p>
    </div>

  </main>
</template>

<script>

import ImageWithSteps from "@/components/ImageWithSteps";
import StepsForBuyingOnALizing from "@/components/StepsForBuyingOnALizing";
import PhysicalPerson from "@/components/PhysicalPerson";
import JuridicaPerson from "@/components/JuridicaPerson";
export default {
  name: 'HomeView',
  components: {JuridicaPerson, PhysicalPerson, StepsForBuyingOnALizing, ImageWithSteps},
}
</script>
