<template>
<!-- start .left-->
<div class="left">
    
    <div class="img-content"><img alt="Foto Claudiomir"  :src="euImage"></div>
               
    <div class="item" >
        <h3><fontawesome class="icon" icon="address-book" /> Contatos</h3>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://api.whatsapp.com/send?phone=5511954112580&text=Ol%C3%A1%20Claudiomir,%20vim%20pelo%20seu%20curr%C3%ADculo.">(11) 95411-2580  <fontawesome icon="mobile-alt" /> </a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="mailto:diomids2@hotmail.com">diomids2@hotmail.com <fontawesome icon="at" /></a></p>
         <p class="link" ><a rel="noopener"  target="_blank" href="mailto:claudiomirneves@gmail.com">claudiomirneves@gmail.com <fontawesome icon="at" /></a></p>
    </div>

    <div class="item" >
        <h3><fontawesome class="icon" icon="network-wired" /> Social</h3>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.linkedin.com/in/claudiomir-neves-de-araujo-078711209/"> linkedin.com/in/claudiomirneves  <fontawesome icon="link" /></a> </p>
</div>

    <div class="item" >
        <h3><fontawesome class="icon" icon="code-branch" /> Code Repositórios</h3>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://github.com/diomids2">github.com/diomids2 <fontawesome icon="link" /></a></p>

    </div>

    <div class="item" >
        <h3><fontawesome class="icon" icon="info" /> Informações Relevantes</h3>
        <p>Inglês Intermediario </p> 
    </div>

        <div class="item" >
        <h3><fontawesome :icon="['fab', 'leanpub']"  /> Cursos Complementares</h3>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=13220127958/12054554">Javaspring Boot – BackEnd <fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=00012445/5830803">Desvendando a Blockchain <fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=00012444/5830803">Desvendando a indrustria  <fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=0009853/5830803">Excel Basico <fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=0007535/5830803">Preparação para o mundo de trabalho<fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=0009854/5830803">Proteção de Dados <fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=0007530/5830803">Segurança do Trabalho<fontawesome icon="link" /></a></p>
        <p class="link" ><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/consulta-certificado?qrcode=0007534/5830803">Economia Circular<fontawesome icon="link" /></a></p>
    </div>
<!-- 
    <div class="item" >
        <h3><fontawesome class="icon" icon="code-branch" />ProjetoAgencia Portfofolio</h3>
        <p class="link link-noprint" ><a rel="noopener"  target="_blank" href="https://nevesdigital.com.br/">Neves Digital Solution<fontawesome icon="link" /></a></p>
        <p class="link link-noprint" ><a rel="noopener"  target="_blank" href="https://claudiomir.nevesdigital.com.br/">Claudiomir Neves Page<fontawesome icon="link" /></a></p>
    </div> -->

</div>
<!-- end .left-->
</template>
<script>
import {mapState} from 'vuex'

 export default{
     name : "Left",
     computed: {
         ...mapState({
             euImage: state => state.euImage 
         })
     }
 }   
</script>