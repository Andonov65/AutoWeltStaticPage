<template>
    <section>
        <div class="mx-md-5 mt-4">
            <h1 class="text-start fs-1">
                <strong>
                    Документација со барање за лизинг: ФИЗИЧКИ ЛИЦА
                </strong>
            </h1>
        </div>
        <p class="fs-5 me-md-5 pe-md-5 my-4">
            Со пополнето барање за одобрување на лизинг,
            <strong>
                профактура на добавувачот
            </strong>
            и
            <strong>
                прифатена лизинг понуда
            </strong>
            , потребно е да се приложат и:
        </p>
        <div class="ms-md-5">
            <ul class="fs-5">
                <li class="ps-md-3" v-for="physicalPerson in physicalPersonList" :key="physicalPerson.text">
                    {{physicalPerson.text}}
                    <a :href="physicalPerson.link" target="_blank">
                        <strong>
                            {{physicalPerson.linkText}}
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
        name: "PhysicalPerson",
        data(){
            return{
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

                ]
            }
        }
    }
</script>

<style scoped>

</style>