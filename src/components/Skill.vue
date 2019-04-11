<template>
  <div
    :class="$mq | mq({xs: 'col-sm-3 col-md-4 text-center', sm: 'col-sm-3 col-md-4 text-center', md: 'col-sm-3 col-md-4 text-center', lg: 'col-sm-3 col-md-4 text-center'})">
    <div
      :class="$mq | mq({xs: 'service-box mt-5 mx-auto', sm: 'service-box mt-5 mx-auto', md: 'service-box mt-5 mx-auto', lg: 'service-box mt-5 mx-auto'})">
      <img :src="skill.name"
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