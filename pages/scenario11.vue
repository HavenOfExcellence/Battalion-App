<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div>
    <ScenarioPage :scenario="11" title="Backup personal data regularly">
      <img src="~/assets/Scam11.png" />
      <h2>
        Every year, about 60 million smart phones are lost, stolen, or damaged.
        Most of us have insurance on our devices, so we are lulled into a false
        sense of security. But if you’ve ever lost your phone, you know it’s the
        data you just can’t replace. Most people would say that their data is
        more important than their device itself, yet only 24% of people say they
        back up their data regularly. What’s more shocking, though, is that 40%
        of people either haven’t backed up their data recently or have never
        backed up their data at all. You know that if you lost all your photos
        and files you’d be a panicked mess. Make backing up your data regularly
        a priority in your life. You can back up to the cloud, to an external
        hard drive, or even to your own computer. Are you prepared to lose all
        your data tomorrow? If not, back it up. This infographic outlines the
        importance of backing up your data as well as some ways to do it. Once
        you’ve made backing up your data a priority, share this infographic with
        your friends. You could be helping someone realize the importance of
        backing up that data.
      </h2>
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
