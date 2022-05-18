<template>
  <div class="w-96 h-96 bg-green-200">
    <Form class="flex-col flex" @submit="onSubmit">
      <FormField name="name"></FormField>
      <FormField name="email" type="email"></FormField>
      <FormField name="password" type="password"></FormField>
    </Form>
  </div>
</template>
<script setup>
import { Form } from "vee-validate";

function onSubmit(values) {
  console.log(values);
}
</script>
