<template lang="html">
    <section :class="[panelClass,cname]">
        <h4>-{{ title }}-</h4>
        <h2>{{title}}</h2>
        <slot></slot>
    </section>
</template>

<script>
    export default {
        props:{
            cname:{
                type:String,
                default:"",
            },
            title:{
                type:String,
                default:"",
            }
        },
        data(){
            return {
                panelClass:"panel"
            }
        }
    }
</script>
