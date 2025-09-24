<script>
    export default { 
        // Add Code Here
        // challenge: use array  
        data(){
            return{
                message:"Choose your fav fruit",
                fruit1: "apple",
                fruit2:"orange",
                fruit3:"peach",

                //use array
                fruits:["apple","orange","peach"]
            }
        }

    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">

        <h3>Using array</h3>
        {{ message }} </br>
        <!--loop through the list using the v-for-->
        <span v-for="fruit in fruits">
              {{ fruit }} <input type="radio" name="fruit">

        </span>
    </div>
</template>

<style scoped>
</style>
