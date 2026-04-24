<template>
    <div>
         <Nav />
         <hr/>
        <PageTitle :pageTitle="pageTitle" />
    </div>
</template>
<script setup>
    const props = defineProps({
        pageTitle:{
            required: true
        }
    })
</script>