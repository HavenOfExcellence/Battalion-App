<script setup>
import { Form, ErrorMessage } from "vee-validate";
function onSubmit(values) {
  console.log("ASDASD");
  console.log(values);
  navigateTo("/scenario2");
}

const schema = {
  answer(value) {
    if (value === undefined) {
      return "Answer is required";
    } else if (value === "1") {
      return "Wrong answer";
    } else {
      return true;
    }
  },
};
</script>

<template>
  <div class="flex flex-col px-5 justify-center items-center">
    <Form
      @submit="onSubmit"
      :validation-schema="schema"
      class="flex flex-col items-start w-full"
    >
      <h4 class="mt-10 text-xl">Question 1 of 5</h4>
      <div class="mt-4 text-2xl">What type of framework is Next.js?</div>
      <div
        class="flex items-center w-full py-4 pl-5 m-2 ml-0 space-x-2 border-2 cursor-pointer bg-gray-200 border-black/10 rounded-xl"
      >
        <FormField
          value="1"
          name="answer"
          type="radio"
          class="w-6 h-6 bg-black"
        />
        <p class="ml-6">ASDASD</p>
      </div>
      <div
        class="flex items-center w-full py-4 pl-5 m-2 ml-0 space-x-2 border-2 cursor-pointer bg-gray-200 border-black/10 rounded-xl"
      >
        <FormField
          value="2"
          name="answer"
          type="radio"
          class="w-6 h-6 bg-black"
        />
        <p class="ml-6">ASDASDasdasd</p>
      </div>
      <ErrorMessage name="answer" />
      <div class="flex justify-between w-full mt-4 text-white">
        <button type="submit" class="w-[49%] py-3 bg-indigo-600 rounded-lg">
          Next
        </button>
      </div>
    </Form>
  </div>
</template>
