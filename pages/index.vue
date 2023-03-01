<template>
  <div>
    <!-- <div>{{ response.details.ext_2 }}</div> -->
    <div>Index</div>
    <div>{{ JSON.stringify(env, null, 2) }}</div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  async asyncData({ $axios, app }) {
    // try {
    //   const response = await $axios.$get(
    //     process.env.BASE_URL + "/rcms-api/4/mission-statement/4"
    //   );
    //   return { response };
    // } catch (e) {
    //   console.log(e.message);
    // }

    // return { url: process.env.BASE_URL + "/rcms-api/4/mission-statement/4" };
    return { env: process.env };
  },
};
</script>
