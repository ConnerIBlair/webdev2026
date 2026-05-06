<template>
    <div>
        <UPageHero class="py-1"/>
        <UPageHeader title="Contact Me!" />


  <UPageSection title="Personal Info">
         <Form label="First Name" />
        <Form label="Middle Initial" />
        <Form label="Last Name" />
  </UPageSection>
    </div>
    <div>
            <UAccordion :items="items" />

    </div>
</template>

<script setup>
    const items = [
  {
    label: 'Are you amazing at coding?',
    content: 'Yes! well, sometimes that is'
  },
  {
    label: 'When are you available for hire?',
    content: 'I will be available for hire starting in May of 2027'
  },
  {
    label: 'Has your day been going well?',
    content: 'It has been going spectacularly, thanks for asking (:'
  }]
</script>