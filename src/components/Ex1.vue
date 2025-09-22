<script>
    export default { 
        // Add Code Here
        data() {
            return {
                message : 'Choose your favorite fruit:',
                // we can also do this with an array. try it out!
                fruit1 : 'apple',
                fruit2 : 'orange',
                fruit3 : 'peach',
                fruits : ['apple', 'orange', 'peach']  // challenge: use array
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
        <h3> Using Array </h3>
        {{ message }} </br>
        <div v-for="fruit in fruits">
            {{ fruit }} <input type="radio" name="fruit">
        </div>
    </div>
</template>

<style scoped>
</style>
