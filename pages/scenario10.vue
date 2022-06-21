<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div>
    <ScenarioPage :scenario="10" title="Dangers of public wifi">
      <img src="~/assets/Scam10.jpg" />
    </ScenarioPage>

    <QuizTemplate
      link="/scenario11"
      question="What are some steps you can take to be safe when connected to public wifi"
      :answers="[
        {
          text: `Check that every website you connect to has https(lock icon) `,
          value: `1`,
        },
        {
          text: `Set your phone to autoconnect to open wifi networks`,
          value: `2`,
        },
        {
          text: `Check banking info quickly so people cannot steal your info`,
          value: `3`,
        },
      ]"
    />
  </div>
</template>

<script setup></script>
