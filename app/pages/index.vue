<template>
    <div>
          <UPageHero
    title="Conner Blair's Website"
    description="Projects get done"
  />

    <UPageSection title="The Clickers">
                  <UPageHero
    :links="links"/>
    </UPageSection>


    <UPageCTA
  title="About Me"
>
<UPageHero
    :links="link"/>
</UPageCTA>

    </div>
</template>

<script setup>
const links = [
        {
        label: "Portfolio", 
        to:"/portfolio"
    },
        {
        label: "Contact", 
        to:"/contact"
    }
]
const link = [
        {
        label: "About Me", 
        to:"/about"
    }]
</script>