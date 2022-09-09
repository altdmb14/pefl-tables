<template>
<div>
    <b-container label="Label">
    <b-row align-v="start">
        <b-col sm="4">1 из 3</b-col>
        <b-col sm="4">2 из 3</b-col>
        <b-col sm="4">3 из 3</b-col>
    </b-row>
    </b-container>
</div>
</template>

<script>
export default {
    data() {
        return {
            email: '',
            items: [
                {age: 41, first_name: 'Abc', last_name: 'Macdonald' }
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