<template>
    
    <ChildComponent :childname="parentname" :clickFunction="alertFunction"/>
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
            parentname:"learning vue step by step"
        }  
    },

    methods:
        {
            alertFunction()
            {
                alert("this is alert");
            }
            
        }
}
</script>