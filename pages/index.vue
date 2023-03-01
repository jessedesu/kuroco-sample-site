<template>
  <div>
    <!-- <div>{{ response.details.ext_2 }}</div> -->
    <div>Index</div>
    <div>{{ url }}</div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  async asyncData({ $axios, app, $config: { baseURL } }) {
    // try {
    //   const response = await $axios.$get(
    //     process.env.BASE_URL + "/rcms-api/4/mission-statement/4"
    //   );
    //   return { response };
    // } catch (e) {
    //   console.log(e.message);
    // }

    // return { url: process.env.BASE_URL + "/rcms-api/4/mission-statement/4" };
    return { url: baseURL };
  },
};
</script>
