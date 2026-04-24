<template>
    <UContainer>
        <!-- Header (nav) -->
        <slot />
        <!-- Footer -->
        <UFooter>
            <template #left>
                      <p class="text-muted text-sm">Copyright Cawno © {{ new Date().getFullYear() }}</p>
            </template>
                <UButton 
                    icon="i-simple-icons-github"
                    variant="outline"
                    size="sm"
                    to="https://github.com/ConnerIBlair"
            />

            <!-- Center -->
                <UNavigationMenu :items="items" variant="link" />

            <template #right>
            </template>

        </UFooter>
    </UContainer>
</template>
<script setup>
const items = [
    {
        label: "Home Page", 
        to:"/"
    },
        {
        label: "About Page change", 
        to:"/about"
    },
        {
        label: "Portfolio", 
        to:"/portfolio"
    },
        {
        label: "Contact", 
        to:"/contact"
    }
]
</script>