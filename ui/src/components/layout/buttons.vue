<template>
<!-- start .btns-->
<div class="btn btn-fixed-lg">

      <!-- #printbtn-->
    <div :v-if="btn" class="" id="print" title="Imprimir" @click="printDoc()" >
         <!-- fas fa-print -->
        <fontawesome icon="print" />
    </div>

     <!-- #email-->
    <div :v-if="btn" class="" id="email" title="Email" onclick="window.location.href='mailto:diomids2@hotmail.com';" >
        <fontawesome icon="envelope" />
    </div>

    <!-- #whatsapp-->
    <a :v-if="btn"  class=""  id="whatsapp" title="Whatsapp" rel="noopener" target="_blank" href="https://api.whatsapp.com/send?phone=5511954112580&text=Ol%C3%A1%20Claudiomir,%20vim%20atrav%C3%A9s%20do%20seu%20curr%C3%ADculo." >
        <!-- fab fa-whatsapp -->
        <fontawesome :icon="['fab', 'whatsapp']"  />
    </a>
  
  
</div>
<!-- end .btns-->
</template>
<script>
import {mapState, mapMutations, mapActions} from "vuex"
 export default{
     name : "Buttons",
    computed: {
        ...mapState({
            msg: state => state.msg,
            btn: state => state.btn,
        })
    },

    methods:{

        ...mapMutations({
            btnMut: 'btn',
        }),

        ...mapActions({
            printDoc: 'printDoc',
        })
    }
 }   
</script>