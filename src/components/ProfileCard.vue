<template>
    <div class="col-lg-3">
        <div class="card border-0 bg-transparent">
        <img :src="image" class="card-img-top rounded-circle" alt="Card image cap" />
        <div class="card-body">
            <h5 class="card-title">{{ title }}</h5>
            <p class="card-text">{{ description }}</p>
            <button @click="handleClick" class="btn btn-transparent text-primary">{{ buttonText }}</button>
        </div>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ProfileCard",
    props: {
      image: {
        type: String,
        required: true,
      },
      title: {
        type: String,
        required: true,
      },
      description: {
        type: String,
        required: true,
      },
      buttonText: {
        type: String,
        default: "Learn More",
      },
    },
    methods: {
      handleClick() {
        this.$emit("button-click");
      },
    },
  };
  </script>
  
  <style scoped>
  .card {
    margin: 20px;
  }
  </style>
  