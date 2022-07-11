<template>
    <section>
        <div class="mt-4">
            <h1 class="text-start fs-1">
                <strong>
                    Документација со барање за лизинг: ПРАВНИ ЛИЦА
                </strong>
            </h1>
        </div>
        <p class="fs-5 me-md-5 pe-md-5 my-4">
            Со пополнето барање за одобрување на лизинг, профактура на добавувачот и
            прифатена лизинг понуда, потребно е да се приложат и:
        </p>
        <div class="ms-md-5">
            <ul class="fs-5">
                <li class="ps-md-3" v-for="jurisdictionPerson in jurisdictionPersonList" :key="jurisdictionPerson.text">
                    {{jurisdictionPerson.text}}
                    <a :href="jurisdictionPerson.link" target="_blank">
                        <strong>
                            {{jurisdictionPerson.linkText}}
                        </strong>
                    </a>
                </li>

            </ul>
        </div>

        <p class="fs-5">
            <strong>
                Документација треба да биде заверена со потпис и печат на овластеното лице!
            </strong>
        </p>

        <p class="fs-5">
            <strong>
                AUTOWELT
            </strong>
            го задржува правото да побара дополнителна документација за разгледување на барањата за одобрување на лизинг.
        </p>

    </section>
</template>

<script>
    export default {
        name: "JuridicaPerson",
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
                ]
            }
        }
    }
</script>

<style scoped>

</style>