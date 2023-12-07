<template>
    <form  class="w-[600px] h-[80px] flex items-center">
        <TextInput type="text" 
        name="textInput"
        class="block w-full mr-2"
        v-model="form.search"
        autocomplete="on"
        placeholder="Search for files and folders" />

    </form>
</template>
<script setup>
import { useForm } from '@inertiajs/vue3';
import TextInput from '@/Components/TextInput.vue';

const form = useForm({
    search: ''
})

</script>
<style scoped>

</style>