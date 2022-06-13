<script setup>
import { array } from "yup";

const props = defineProps({
  question: {
    type: String,
    default: "How are you?",
  },
  options: {
    type: array,
    default: ["Yes", "No", "Okay"],
  },
});
const { questions, options } = props;
</script>

<template>
  <div class="w-full h-full">
    <h2 class="text-sm font-semibold text-gray-800 mt-6 mb-8">Question</h2>
    <li>
      <label class="block font-semibold whitespace-pre-wrap">asdasd</label>
    </li>
  </div>
</template>
