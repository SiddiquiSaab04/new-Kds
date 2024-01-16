<template>
    <ul class="modifiers pl-4">
        <li  v-for="(modifier, index) in modifiers" :key="index" :modifier="modifier" >{{ modifier }}</li>
       
    </ul>
</template>
<script>
export default {
    props: ["modifiers"],
    name:'ModifiersComponent'
}

</script>
<style>

</style>