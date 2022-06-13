<script setup>
import { Field, ErrorMessage } from "vee-validate";
import { boolean } from "yup";

const props = defineProps({
  label: {
    type: String,
    default: "",
  },
  name: {
    type: String,
    default: "",
  },
  type: {
    type: String,
    default: "text",
  },
  rules: {
    type: Function,
    default: null,
  },
  placeholder: {
    type: String,
    default: "",
  },
  value: {
    type: String,
    default: "",
  },
  disable: {
    type: boolean,
    default: false,
  },
});

const { placeholder, disabled, rules, label, name, type, value } = props;

function returnfalse() {
  return false;
}
</script>

<template>
  <Field
    :name="name"
    :type="type"
    :placeholder="placeholder"
    :rules="rules"
    :change="change"
    :value="value"
    :disable="disable"
  />
  <ErrorMessage v-if="disabled" name="name" />
</template>
