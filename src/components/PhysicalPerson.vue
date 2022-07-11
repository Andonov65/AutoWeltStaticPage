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
        props: {
            physicalPersonList: {
                type: Array
            }
        }
    }
</script>

<style scoped>

</style>