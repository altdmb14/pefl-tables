<template>
<div>
    <b-container label="Label">
    <b-row align-v="start">
        <b-col>
        <b-table striped hover :items="items"></b-table>
        </b-col>
    </b-row>
    </b-container>
</div>
</template>

<script>
export default {
    data() {
        return {
            fields: ['Игрок', 'first_name', 'last_name'],
            email: '',
            items: [
                {Игрок: 41, first_name: 'Abc', last_name: 'Macdonald' }
            ]
        }
    },
    methods: {
        addNewRow(){
            console.log("test"),
            this.items.push({age: 12, first_name: 'Art', last_name: 'New' });
        }
    },
}
</script>