<template>
  <nav class="navbar navbar-expand-lg navbar-primary bg-primary">
    <div class="container-fluid mx-5">
      <a class="navbar-brand inter-tight text-white" href="#">
        <img src="https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" alt="" width="30" height="24" class="d-inline-block align-text-top">
        Vue JS
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active inter-tight text-white" aria-current="page" href="#hero">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active inter-tight text-white" aria-current="page" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active inter-tight text-white" aria-current="page" href="#profile">Profile</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active inter-tight text-white" aria-current="page" href="#blog">Blog</a>
          </li>
        </ul>
        <form class="d-flex">
          <input class="form-control me-2 inter-tight text-white" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-success inter-tight text-white" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
