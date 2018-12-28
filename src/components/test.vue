<template>
    <div :class="this.$options.name">    
        <div class="search">
            <input type="text" class="search__input" placeholder="Buscar..." v-model="busqueda">
            <button class="button search__button" @click="showModal">Buscar</button>
        </div>
        <!--<ul>
            <li v-for="(items,i) in appointments" v-bind:key="i">
                <span>Dueño:</span>
                 {{items.petOwner}}
            </li>
        </ul>-->
    </div>
</template>

<script>

export default {
    name: "content-search",
    data() {
        return{
            //appointments: apts
            busqueda: ''
        }
    },
    methods: {
        showModal: function(){
            //console.log('Mostrando Modal');   
            console.log(`Buscando: ${this.busqueda}`);   
        }
    }
    
}
</script>

<style lang="scss" scoped>

@import '~styles/main';

button, input{
    border:none;
    outline: none;
}

.search{
   display: flex; 
   max-width: 500px;
   width: 100%;
   margin: 0 auto;
   &__input{
       padding: 10px;
       border: 1px solid #8b8686;
       flex: 2;
       transition: all 0.4s;
       color: $red-color;
       &:focus{
           box-shadow: 0 0 10px #927e7e;
       }
   }
   &__button{
       background-color: #000;
       color:#fff;
       border:1px solid #000;
       flex: 1;
       cursor: pointer;
       transition: all 0.4s;
       &:hover{
            background-color: #fff;
            color:#000;
       }
   }
}
/* 
https://markus.oberlehner.net/blog/how-the-bem-css-naming-scheme-can-improve-vue-component-architecture/
vue js webpack structure
https://www.awwwards.com/websites/vue-js/
https://clubwuf.pe/
https://bolsadetrabajo.laborum.pe/bcp/another-work-positions.html
https://laborum.pe/p/buscar-ofertas
https://www.samsung.com.pe/noche-magica/#/ --VUE JS
https://landing.mapfre.com.pe/trebol-salud/?utm_source=facebook_aon&utm_medium=linkad_lal2%25rmkt&utm_campaign=trebol&utm_content=noviembre-mapa&fbclid=IwAR2MCpqofEESwpF35CMnZqbsvnzZx7hFXg-VefORZ7dBhsWgEZn61bdFOqs
http://posgrado.pucp.edu.pe/admision/programas-en-convocatoria/?buscar=Maestria+en+informatica
https://www.campusromero.pe/?utm_source=social-facebook&utm_medium=trafico-cpc&utm_campaign=grati-locura-chica-empresas&fbclid=IwAR05f33W5iP9dAjTAWLa4lBVEt7tA0e79YGGRpauWzJLVUGJNOIBoQGQfXw
https://unagrancompania.com/?utm_source=TomadeCanal&utm_medium=ElComercio&utm_campaign=Aniversario#queremos-celebrar
https://www.coronasunsets.pe/agegate?destination=?utm_source=BRIGHTROLL&utm_medium=vid&utm_campaign=PRE%20SUMMER&utm_content=TRACKER%20PRESUMMER
https://www.samsung.com.pe/regala-galaxy
https://www.independencia.com.pe/
https://www.netflix.com/pe/#this-is-netflix

*/

</style>

