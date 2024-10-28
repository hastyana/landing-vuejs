<template>
    <div class="col-lg-4">
        <div class="card bg-transparent">
          <img :src="image" class="card-img-top bg-secondary" alt="Card image cap" />
          <div class="card-body text-start">
            <h5 class="card-title">{{ title }}</h5>
            <p class="card-text my-4">{{ description }}</p>
            <button @click="handleClick" class="btn btn-primary">{{ buttonText }}</button>
          </div>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "BlogCard",
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
  