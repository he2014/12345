<template type="html">
   <div class="boxGroup-class">
     <slot >
     </slot>
   </div>

</template>

<script type="text/javascript">
  export default {
    model:{

    },
    props:{
        value:[],
    },
    watch:{
      value:(newValue,oldValue)=>{
        console.log(newValue+"------------------"+oldValue);
      }
    },
    mounted(){
      this.$on("fromCheck",(value) => {
            alert(value);
      })
    },
     data(){
         return {
            // console.log("dasd");
         }
     },
     methods:{
        // this.$broadcast( 'addChildDataEvent', self.dataInput )
     }
  }
</script>
<style lang="scss">


</style>
