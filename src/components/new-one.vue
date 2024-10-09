<template>
    <!-- {{ 2+2 }} refers to calculate 2+2 so result = My 4 vue projcet -->
    <h1>My {{ 2 + 2 }} vue project</h1>
    <!-- Display length of character -->
    <h1>Length of Hello = {{ "Hello".length }}</h1>
    <h1>My email : {{ email = "aaa@gmail.com"}}</h1> <!-- we can asign value after property so old value can't display-->
    <h1>My name is {{ myName() }}</h1>
</template>

<script>
export default {
    name: "PAGES", // name is property to call in file App.vue to define components
    data() {
        return {
            email: 'abc@gmail.com ',
            // And we can use callback function
            myName: function () {
                return "Somonor"
            }
        }
    },
    

}
</script>
<style scoped>
h1 {
    color: rebeccapurple;
}
</style>