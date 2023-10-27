<template>
    <div>
        <h1> {{ pageTitle }}</h1>
        <ul>
            <ListItem
                v-for="item in list"
                :key="item"
                :item="item"
            />
        </ul>
    </div>
</template>

<script>
import  ListItem from "./ListItem"

export default {
    name: "GroceryList",
    components: {
        ListItem
    },
    data() {
        return {
            list: ['pommes', 'bananes', 'cerises'],
            pageTitle:'Ma liste de courses'
        }
    }

}
</script>
