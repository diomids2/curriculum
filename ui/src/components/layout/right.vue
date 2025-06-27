<template>
<!-- start .right-->
<div class="right">
    <div class="img-content"><img alt="Foto Claudiomir"  :src="euImage"></div>

    <div class="item">
        <h1>Claudiomir Neves de Araujo</h1> 
    </div>

    <div class="item" >
        <h3><fontawesome icon="graduation-cap" /> Formação</h3>
        <p><a rel="noopener"  target="_blank" href="https://www.sp.senai.br/curso/tecnico-em-desenvolvimento-de-sistemas/99222"> Técnico em Desenvolvedor de Sistema | SENAI | <small>2019-2021</small><fontawesome icon="link" /></a></p>
    </div>

    <div class="item" >
        <h3><fontawesome :icon="['fab', 'leanpub']"  /> Conhecimentos</h3>
        <ul>
            <li>Front-End
                <p>HTML, CSS, JavaScript e Frameworks como VueJs, React.JS</p>
            </li>
            <li>Banco de Dados 
                <p>SQL Server e Mysql </p>
            </li>
            <li>Ferramentas
                <p>Git, Npm e Trello</p>
            <li>Web Designer
                <p>Wordpress com Elementor Pro</p>
            </li>
            <li>Designer
                <p>UX/UI, Figma e Photoshop avançado</p>
            <li>Informatica em geral
                <p>Microsoft Office, Recuperação de dados (Backup), Solução de problemas de hardware e software, redes, administração de sistemas, reparos, suporte técnico </p>
        
            </li>
        </ul>              
    </div>

    <div class="item" >
        <h3 class="no-print"><fontawesome icon="briefcase" /> Experiências Anteriores</h3>
        <ul class="experiencias">
            <li v-for="(xp, i) in experiencias" :key="i" :class="{'no-print': i > 0}" > 
                <h4>{{xp.empresa.toUpperCase()}}</h4>
                <h5>{{xp.cargo}} | <small>{{xp.periodo}}</small> </h5>
                <p v-for="(descricao, d) in xp.descricao" :key="d">{{descricao}}</p>
            </li>
        </ul>
        <small class="no-screen">Para mais acesse:<br/> <b>diomids2.github.io/curriculum</b></small>            
    </div>

    <div class="item" >
        <h3><fontawesome icon="dollar-sign" /> Pretenção Salarial</h3>
        <p>A combinar.</p>
    </div> 

    <div class="item" >
        <h3><fontawesome icon="bullseye" /> Objetivo</h3>
        <p>
            Tenho como objetivo desempenhar com o máximo de qualidade e aprender cada dia mais nesse imenso mundo que é a Inteligencia da Informação. <br>
        </p>
    </div>
</div>
<!-- end .right-->
</template>
<script>
import {mapState} from 'vuex'
 export default{
     name : "Right",
     computed: {
        ...mapState({
            euImage: state => state.euImage,
            experiencias: state => state.experiencias
        })
     }
 }   
</script>