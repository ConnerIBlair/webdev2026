<template>
    <div>
        <Header pageTitle="Contact" />
        <UForm @submit="processForm">
            <UFormField label="First Name">
                <UInput v-model="firstName">
                </UInput>
            </UFormField>
            <UButton type="submit"> Submit</UButton>
        </UForm>
        <div v-if="submitted == true">
            Hi, my first name is {{ submittedFirstName }}
        </div>
    </div>
</template>

<script setup>
    const firstName = ref('')
    const submitted = ref(false)
    const submittedFirstName = ref('')
    function processForm(event){
        submittedFirstName.value = firstName.value;
        submitted.value = true;
        firstName.value = ''; // Reset the input field

        alert(`Hi ${submittedFirstName.value}`)
    }
</script>