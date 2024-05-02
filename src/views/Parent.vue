<template>
    <ChildComponent :childname="parentname" :clickFunction="alertFunction"/>
    <button v-on:click="incount">click me</button>  
</template>
<script>
import ChildComponent from "../components/Child.vue"
export default{
    name:'Parent',
    components:{
        ChildComponent
    },
    data()
    {
        return{
            parentname:"learning vue step by step",
            count:0
        }  
    },

    methods:
        {
            alertFunction()
            {
                alert("this is alert");
            },
            incount(){
                this.count =10;
                console.log(this.count);
            }
            
        }
}
</script>