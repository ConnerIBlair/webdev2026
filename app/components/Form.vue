<template>
    <div>
        <Header pageTitle="Contact" />
        <UForm @submit="processForm">
            <UFormField :label="props.label">
                <UInput v-model="firstName">
                </UInput>
            </UFormField>
            <UButton type="submit"> Submit</UButton>
        </UForm>
        <div v-if="submitted == true">
            Hi, my name is {{ submittedFirstName }}
        </div>
    </div>
</template>

<script setup>

    const props = defineProps({
  label: {
    type: String,
    default: 'First Name'
  }
})

    const firstName = ref('')
    const submitted = ref(false)
    const submittedFirstName = ref('')

    const firstNameLabel = ref('First Name')

    function processForm(event){
        submittedFirstName.value = firstName.value;
        submitted.value = true;
        firstName.value = ''; // Reset the input field

        // alert(`Hi ${submittedFirstName.value}`)
    }
</script>