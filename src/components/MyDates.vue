<template>
    <div class="datesContainer">
        <div v-for="(date, index) in dates" :key="index" class="singleDate">
            <p>{{date}}</p> 
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyDates',
    props: {
        dates: Array
    }
}
</script>

<style scoped lang="scss">
    .singleDate {
        background-color: #4d4d4d;
        padding: 0.5rem;
        margin-bottom: 1rem;
        width: 100%;

        p {
            color: #ea4a56;
        }
    }
</style>