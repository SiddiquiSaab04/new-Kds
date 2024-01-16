<template>

    <li class="lists pl-4 pt-3 font-semibold">{{list.uantity}}x {{list.product}}</li>
    <modifiers-component-vue :modifiers="list.modifiers"/>
</template>
<script>
import ModifiersComponentVue from '../components/ModifiersComponent.vue'

export default {

    props: ["list"],
    name:'ListComponent',
    components:{
    ModifiersComponentVue
    }
}

</script>
<style>
.lists{
   
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;

}
</style>