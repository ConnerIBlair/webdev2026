<template>
    <article class=" flex-1 p-6 rounded-xl" :class="className">
    <div class="font-bold text-xl">{{title}}</div>
    <div>
    
        
    </div>
    </article>
</template>
<script setup>
    const props = defineProps({
        title:{
            default: 'Title'
        },
        body:{
            default: ' '
            },
        className:{
            default:'bg-gray-800'
        }
    })
</script>