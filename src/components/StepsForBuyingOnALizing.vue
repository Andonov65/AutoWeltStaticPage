<template>
    <section>
        <h1 class="mb-5">
            <strong>Чекори за купување возило на лизинг:</strong>
        </h1>
        <div class="ms-md-5 fs-5">
            <ol>
                <li v-for="step in stepsForLizingList" :key="step.stepName" class="mb-3">
                    <div class="fs-3">
                        {{step.stepName}}
                    </div>
                    <div>
                        {{step.stepDescription}}
                    </div>
                    <strong>
                        {{step.stepRemark}}
                    </strong>
                </li>
            </ol>
        </div>
    </section>
</template>

<script>
    export default {
        name: "StepsForBuyingOnALizing",
        props: {
            stepsForLizingList: {
                type: [],
                required: false
            }
        }
    }
</script>

<style scoped>

</style>