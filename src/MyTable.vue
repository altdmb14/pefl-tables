<template>
<div>
<h3>Скиллы</h3>
<table align="center" style="border 1px solid red;">

<thead style="border 1px solid red;">
<tr>
<th rowspan="3">№</th>
<th rowspan="3">ИГРОК</th>
<th colspan="5">КАЧЕСТВА</th>
</tr>

<tr> 
<th colspan="3">Ходовые</th>
<th colspan="2">Ударные</th>
</tr>

<tr> 
<th>Мощь</th>
<th>Скорость</th>
<th>Дриблинг</th>
<th>Удар</th>
<th>Дальн.удар</th>
</tr>
</thead>

<tbody style="text-align: center;">
<tr v-for="row in rows">
    <td>{{row.number}}</td>
    <td>{{row.name}}</td>
    <td>{{row.power}}</td>
    <td>{{row.speed}}</td>
    <td>{{row.dribling}}</td>
    <td>{{row.udar}}</td>
    <td>{{row.dudar}}</td>
</tr>
</tbody>

</table>

</div>
</template>

<script>
export default {
    data () {
        return {
            rows: [
                {number: 29, name: 'Булут', power: 8, speed: 3, dribling: 5, udar: 1, dudar: 2},
                {number: 25, name: 'Кармазиненко', power: 6, speed: 1, dribling: 6, udar: 4, dudar: 5},
                {number: 12, name: 'Давтян', power: 3, speed: 1, dribling: 6, udar: 5, dudar: 7},
                {number: 28, name: 'Вайнбергер', power: 5, speed: 3, dribling: 5, udar: 7, dudar: 6},
                {number: 27, name: 'Мусона', power: 9, speed: 5, dribling: 5, udar: 3, dudar: 5},
                {number: 31, name: 'Мойзер', power: 4, speed: 4, dribling: 3, udar: 6, dudar: 5},
                {number: 13, name: 'Кодзава', power: 5, speed: 5, dribling: 2, udar: 7, dudar: 4},
                {number: 26, name: 'Булатов', power: 4, speed: 1, dribling: 7, udar: 7, dudar: 6},
                {number: 10, name: 'Веллинг', power: 9, speed: 1, dribling: 5, udar: 8, dudar: 4},
                {number: 11, name: 'Алиев', power: 4, speed: 5, dribling: 3, udar: 8, dudar: 4},
            ]
        }
    },
}
</script>

<style>
table {
    font-family: 'Open Sans',
    sans-serif;
    width: 750px;
    border-collapse: collapse;
    border: 1px solid red;
    margin: 10px 10px 0 10px;
}

td {
   text-align: "center";
}

th {
   border: 1px solid red;
}

table th {
    text-align: center;
    background: #44475C;
    color: #FFF;
    padding: 8px;
    min-width: 1px;
}

table td {
    padding: 8px;
    border-right: 1px solid red;
}

table td:last-child {
    border-right: none;
}

table tbody tr:nth-child(2n) td{
    background: #D4D8F9;
}
</style>