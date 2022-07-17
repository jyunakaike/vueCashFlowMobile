<template>
    <Layout>
        <template #header>
            <Header></Header>
        </template>
        <template #resume>
            <Resume :total-label="'Ahorro total'" :label="label" :total-amount="1000" :amount="amount">
                <template #graphic>
                    graphic
                </template>
                <template #action>
                    action
                </template>
            </Resume>
        </template>
        <template #movements>
            <Movements :movements="movements" />
        </template>
    </Layout>
</template>

<script>
import Layout from "./Layout.vue";
import Header from "./Header.vue";
import Resume from "./Resume";
import Movements from "./Movements/Index.vue";

export default {
    components: {
        Layout,
        Header,
        Resume,
        Movements,
    },
    data() {
        return {
            label: null,
            amount: null,
            movements: [{
                id: 0,
                title: "Movimiento 1",
                description: "Lorem ipsum",
                amount: 1000,
            }, {
                id: 1,
                title: "Movimiento 2",
                description: "Lorem ipsum",
                amount: 1000,
            }, {
                id: 3,
                title: "Movimiento 3",
                description: "Lorem ipsum",
                amount: 1000,
            }, {
                id: 4,
                title: "Movimiento 4",
                description: "Lorem ipsum",
                amount: 1000,
            }, {
                id: 5,
                title: "Movimiento 5",
                description: "Lorem ipsum",
                amount: 1000,
            }, {
                id: 6,
                title: "Movimiento 6",
                description: "Lorem ipsum",
                amount: 1000,
            }]
        }
    }
}
</script>

<style>
</style>