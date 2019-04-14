<template>
  <div
    :class="$mq | mq({xs: 'col-6 text-center d-flex justify-content-center align-items-center', sm: 'col-6 text-center d-flex justify-content-center align-items-center', md: 'col-1 text-center d-flex justify-content-center align-items-center', lg: 'col-1 text-center d-flex justify-content-center align-items-center'})">
    <div
      :class="$mq | mq({xs: 'service-box mt-1', sm: 'service-box mt-1', md: 'service-box mt-1', lg: 'service-box mt-1'})">
      <img :src="skill.url" :class="$mq | mq({xs: 'pt-3', sm: 'pt-3', md: 'pt-3', lg: 'pt-3'})" :id="skill.id">
    </div>
  </div>
</template>

<script>
  export default {
    name: "skill",
    props: ["skill"],
    data() {
      return {};
    },
    computed: {},
    methods: {},
    components: {}
  };
</script>