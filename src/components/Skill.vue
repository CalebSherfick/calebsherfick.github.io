<template>
  <div
    :class="$mq | mq({xs: 'col-6 text-center', sm: 'col-6 text-center', md: 'col-4 text-center', lg: 'col-4 text-center'})">
    <div
      :class="$mq | mq({xs: 'service-box mt-5 mx-auto', sm: 'service-box mt-5 mx-auto', md: 'service-box mt-5 mx-auto', lg: 'service-box mt-5 mx-auto'})">
      <img :src="skill.url"
        :class="$mq | mq({xs: 'skill-img pt-3', sm: 'skill-img pt-3', md: 'skill-img pt-3', lg: 'skill-img pt-3'})">
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