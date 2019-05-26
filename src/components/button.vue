<template>
    <button class=aw-button :disabled=disabled :class="{'is-round':round}">
        <slot></slot>
    </button>
</template>
<style scoped>
    .aw-button{
        padding:0 1em;
        border: 1px solid #e0e0e0
    }
    .aw-button.is-round{
        border-radius: 5px
    }
</style>
<script>
    export default{
        name: 'awButton',
        props:{
            disabled: Boolean,
            round: Boolean
        }
    }
</script>