<template>
    <h3>Welcome to {{ childname }}</h3>
    <button v-on:click="clickFunction">Click Here</button>
</template>
<script>
export default{
    name:'ChildComponent',

    //dynamically var call
    props:{
        childname:String,
        clickFunction: Function
    }
}
</script>