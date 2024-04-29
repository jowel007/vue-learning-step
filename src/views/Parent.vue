<template>
    <h2>This is Parent COmponent</h2>
    <ChildComponent />
</template>
<script>
import ChildComponent from "../components/Child.vue"
export default{
    name:'Parent',
    components:{
        ChildComponent
    }
}
</script>