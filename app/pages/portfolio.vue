<template>
    <div>
        <UPageHeader title="Projects done and in the works" />
                <UPageSection class="py-1">
        <UCarousel v-slot="{ item }" :items="items" :ui="{ item: 'basis-1/3' }">
            <img :src="item" width="234" height="123" class="rounded-lg" loading="fast">
        </UCarousel>
        </UPageSection>
                        
    </div>
</template>
<script setup>
const items = [
  "/Images/Cover.jpg",
  '/Images/Cassonia.png',
  '/Images/Mookie%20Banner.png',
  '/Images/image.png',
  'https://picsum.photos/468/468?random=5'
]
</script>