<template>
    <div>
        <select v-model="selected" class="form-select mt-10 block w-full border p-3 rounded">
        <option value="0" disabled>Select Country</option>
        <option v-for="country in countries" :value="country.ID">{{country.Country}}</option>
        </select>
    </div>
</template>

<script>
    export default {
        name:"CountrySelect",
        props:['countries'],
        data(){
            return{
                selected:0
            }
        }
    }
</script>