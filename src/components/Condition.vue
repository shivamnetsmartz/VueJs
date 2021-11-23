<template>
    <div>
        <h1 v-if="show"> Conditional Rendering in Vue Js</h1>
    </div>
</template>

<script>
export default {
    name:"Condition",
    data(){
    return{
        show:true
    }
}
}
</script>