<template>
  <main class="container mx-md-auto font-style">
      <image-with-steps/>
      <steps-for-buying-on-a-lizing :steps-for-lizing-list="stepsForLizingList"/>
      <physical-person :physical-person-list="physicalPersonList" />
      <hr/>
      <juridica-person :list-jurisdiction-person="jurisdictionPersonList"/>
      <hr/>
      <p class="text-danger fs-5 me-md-5 pe-md-5">
          <i>
              * НАПОМЕНА: ДОКОЛКУ ПОДАТОЦИТЕ КОИ ГИ ОСТАВАТЕ ПРИ ПРЕД-ОДОБРУВАЊЕТО НЕ СЕ ТОЧНИ И ПРЕЦИЗНИ МОЖНО Е АПЛИКАЦИЈАТА ЗА ЛИЗИНГ ДА ВИ БИДЕ ОДБИЕНА ИЛИ ПРОЛОНГИРАНА ОД СТРАНА НА БАНКАТА И ПРИТОА ГО ГУБИТЕ ОСТАВЕНИОТ КАПАР.
          </i>
      </p>
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
    data(){
      return{
          jurisdictionPersonList: [
              {
                  text: "Барање за одобрување на лизинг",
                  linkText: "(превземи барање)",
                  link: "https://s-leasing.mk/content/%D0%91%D0%B0%D1%80%D0%B0%D1%9A%D0%B5%20%D0%B7%D0%B0%20%D0%BE%D0%B4%D0%BE%D0%B1%D1%80%D1%83%D0%B2%D0%B0%D1%9A%D0%B5%20%D0%BD%D0%B0%20%D0%BB%D0%B8%D0%B7%D0%B8%D0%BD%D0%B3_Pravni%20Lica-11.01.2022.pdf"
              },
              {
                  text: "Копија од тековна состојба, не постара од 6 недели",
                  linkText: "",
                  link: ""
              },
              {
                  text: "Завршна сметка (биланс на состојба и биланс на успех за последните две фискални години)",
                  linkText: "",
                  link: ""
              },
              {
                  text: "Аналитички заклучни листови кон завршните сметки за последните две години",
                  linkText: "",
                  link: ""
              },
              {
                  text: "Аналитички заклучен лист за тековната година со последен датум на книжење",
                  linkText: "",
                  link: ""
              },
              {
                  text: "ИСогласност за извадок од Македонско Кредитно Биро",
                  linkText: "(превземи согласност)",
                  link: "https://s-leasing.mk/content/%D0%A1%D0%BE%D0%B3%D0%BB%D0%B0%D1%81%D0%BD%D0%BE%D1%81%D1%82%20%D0%B7%D0%B0%20%D0%B8%D0%B7%D0%B2%D0%B0%D0%B4%D0%BE%D0%BA%20%D0%BE%D0%B4%20%D0%9C%D0%B0%D0%BA%D0%B5%D0%B4%D0%BE%D0%BD%D1%81%D0%BA%D0%BE%20%D0%9A%D1%80%D0%B5%D0%B4%D0%B8%D1%82%D0%BD%D0%BE%20%D0%91%D0%B8%D1%80%D0%BE.pdf"
              },
              {
                  text: "Изјава за вистински сопственик",
                  linkText: "(превземи согласност)",
                  link: "https://s-leasing.mk/content/Izjava-za-vistinski-sopstvenik.pdf"
              },
          ],
          physicalPersonList: [
              {
                  text: "ПРОФАКТУРА",
                  linkText: "",
                  link: ""
              },
              {
                  text: "БАРАЊЕ за одобрување на лизинг ",
                  linkText: "(превземи барање)",
                  link: "https://s-leasing.mk/content/%D0%91%D0%B0%D1%80%D0%B0%D1%9A%D0%B5%20%D0%B7%D0%B0%20%D0%BE%D0%B4%D0%BE%D0%B1%D1%80%D1%83%D0%B2%D0%B0%D1%9A%D0%B5%20%D0%BD%D0%B0%20%D0%BB%D0%B8%D0%B7%D0%B8%D0%BD%D0%B3-Fizicki%20Lica.pdf"
              },
              {
                  text: "Копија од ЛИЧНА КАРТА",
                  linkText: "",
                  link: ""
              },
              {
                  text: "ПОТВРДА од работодавецот за редовен работен однос",
                  linkText: "",
                  link: ""
              },
              {
                  text: "Административна забрана од плата од работодавецот",
                  linkText: "(превземи Административна забрана)",
                  link: "https://s-leasing.mk/content/%D0%90%D0%B4%D0%BC%D0%B8%D0%BD%D0%B8%D1%81%D1%82%D1%80%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%B0%20%D0%B7%D0%B0%D0%B1%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D0%B4%20%D0%BF%D0%BB%D0%B0%D1%82%D0%B0%20%D0%BE%D0%B4%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BE%D0%B4%D0%B0%D0%B2%D0%B5%D1%86%D0%BE%D1%82%20%D0%B2%D0%BE%20%D0%BA%D0%BE%D1%80%D0%B8%D1%81%D1%82%20%D0%BD%D0%B0%20%D0%A8%D0%9F%D0%90%D0%A0%D0%9A%D0%90%D0%A1%D0%95%20%D0%9B%D0%98%D0%97%D0%98%D0%9D%D0%93%20%D0%94%D0%9E%D0%9E%20%D0%A1%D0%BA%D0%BE%D0%BF%D1%98%D0%B5.pdf"
              },
              {
                  text: "ИЗЈАВА за редовна отплата",
                  linkText: "(превземи Изјава)",
                  link: "https://s-leasing.mk/content/%D0%98%D0%B7%D1%98%D0%B0%D0%B2%D0%B0%20%D0%B7%D0%B0%20%D1%80%D0%B5%D0%B4%D0%BE%D0%B2%D0%BD%D0%B0%20%D0%BE%D1%82%D0%BF%D0%BB%D0%B0%D1%82%D0%B0.pdf"
              },
              {
                  text: "Годишна даночна пријава (доколку барателот остварува дополнителни приходи)",
                  linkText: "",
                  link: ""
              },
              {
                  text: "Декларации за прием за бруто плата за последните 3 месеци",
                  linkText: "",
                  link: ""
              },
              {
                  text: "СОГЛАСНОСТ за извадок од Македонско Кредитно Биро",
                  linkText: "(превземи согласност)",
                  link: "https://s-leasing.mk/content/%D0%A1%D0%BE%D0%B3%D0%BB%D0%B0%D1%81%D0%BD%D0%BE%D1%81%D1%82%20%D0%B7%D0%B0%20%D0%B8%D0%B7%D0%B2%D0%B0%D0%B4%D0%BE%D0%BA%20%D0%BE%D0%B4%20%D0%9C%D0%B0%D0%BA%D0%B5%D0%B4%D0%BE%D0%BD%D1%81%D0%BA%D0%BE%20%D0%9A%D1%80%D0%B5%D0%B4%D0%B8%D1%82%D0%BD%D0%BE%20%D0%91%D0%B8%D1%80%D0%BE.pdf"
              },
          ],
          stepsForLizingList: [
              {
                  stepName: "ИЗБЕРЕТЕ ГО ВОЗИЛОТО",
                  stepDescription: "Најпрво го избирате возилото кое сакате да го купите и добивате понуда за истото. Според изборот и понудата се подготвуваат потребните документи.",
                  stepRemark: ""
              },
              {
                  stepName: "НАШИТЕ ВРАБОТЕНИ ЌЕ ВИ ГИ ПОБАРААТ ПОТРЕБНИТЕ ПОДАТОЦИ",
                  stepDescription: "Ги оставате сите потребни податоци на нашите вработени за да ја подготват целокупната документација која е потребна за аплицирање за лизингот.",
                  stepRemark: ""
              },
              {
                  stepName: "ПРЕДОДОБРУВАЊЕ",
                  stepDescription: "Според податоците се преминува на фазата за пред-одобрување која ги елиминира или намалува можностите да бидете одбиени. Затоа е потребно податоците кои ќе ги оставите да бидат точни и прецизни. Лизинг копманијата ја разгледаува вашата апликација и дололку се е во ред ќе Ви го одобрат лизингот и ќе ве известат за тоа. Дополнително ќе ви ги кажат понатамошните чекори.",
                  stepRemark: ""
              },
              {
                  stepName: "КАПАР",
                  stepDescription: "   Доколку помине постапката на пред-одобрување потребно е да оставите капар за избраното возило за да Ви биде резервирано се до конечно одобрувањето од банката.",
                  stepRemark: ""
              },
              {
                  stepName: "ПРЕЗЕМАЊЕ НА ВОЗИЛОТО",
                  stepDescription: "Откако ќе се завршите целата процедура и лизингот ќе биде одобрен се договара датумот за превземање на возилото.",
                  stepRemark: "НАПОМЕНА: Пред превземање на возилото потребно е да обезбедите КАСКО ПОЛИСА."
              },
          ]
      }
    }

}
</script>
