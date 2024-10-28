<script setup>
import BlogCard from '@/components/BlogCard.vue';
import BrandSlide from '@/components/BrandSlide.vue';
import Footer from '@/components/Footer.vue';
import Navbar from '@/components/Navbar.vue';
import ProfileCard from '@/components/ProfileCard.vue';
</script>

<template>
    <Navbar />

    <!-- Hero Section -->
    <div id="home" class="container my-5 py-5">
        <div class="row">
            <div class="col-lg-6">
                <div class="lc-block mb-3">
                    <div editable="rich">
                        <h2 class="fw-bold display-5 text-start inter-tight">
                            Lorem Ipsum Dolor Sit Amet
                        </h2>
                        <p class="lead text-start inter-tight mt-3">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra.
                        </p>
                    </div>
                </div>
                <div class="lc-block d-grid gap-2 d-md-flex justify-content-md-start">
                    <a class="btn btn-primary px-4 me-md-2" href="#" role="button">Get Started</a>
                </div>
            </div>
            <div class="col-lg-6">
                <img src="https://images.unsplash.com/photo-1530435460869-d13625c69bbf?crop=entropy&amp;cs=tinysrgb&amp;fit=crop&amp;fm=jpg&amp;ixid=MnwzNzg0fDB8MXxzZWFyY2h8MTB8fHdlYnNpdGV8ZW58MHwwfHx8MTYyMTQ0NjkyNg&amp;ixlib=rb-1.2.1&amp;q=80&amp;w=1080&amp;h=768" class="d-block mx-lg-auto img-fluid" alt="" loading="lazy">
            </div>
        </div>
    </div>

    <!-- Fetured Section -->
    <div class="bg-primary">
        <div class="container my-5 py-5">
            <div class="col-lg">
                <div class="lc-block mb-5">
                    <div editable="rich">
                        <h2 class="fw-semibold display-6 text-center inter-tight text-white">
                            Feature Brand
                        </h2>
                    </div>
                </div>
            </div>
            <BrandSlide />
        </div>
    </div>

    <!-- About Section -->
    <div id="about" class="container my-5 py-5">
        <div class="row">
            <div class="col-lg-6">
                <img src="https://images.unsplash.com/photo-1530435460869-d13625c69bbf?crop=entropy&amp;cs=tinysrgb&amp;fit=crop&amp;fm=jpg&amp;ixid=MnwzNzg0fDB8MXxzZWFyY2h8MTB8fHdlYnNpdGV8ZW58MHwwfHx8MTYyMTQ0NjkyNg&amp;ixlib=rb-1.2.1&amp;q=80&amp;w=1080&amp;h=768" class="d-block mx-lg-auto img-fluid" alt="" loading="lazy">
            </div>
            <div class="col-lg-6">
                <div class="lc-block mb-3">
                    <div editable="rich">
                        <p class="lead text-start inter-tight fw-bold ">
                            About
                        </p>
                        <h2 class="fw-bold display-5 text-start inter-tight">
                            Lorem ipsum dolor sit amet
                        </h2>
                        <div class="lc-block d-grid gap-2 d-md-flex justify-content-md-start my-3">
                            <a class="btn btn-primary px-4 me-md-2" href="#" role="button">Get Started</a>
                        </div>
                        <p class="lead text-start inter-tight mt-3">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Profile Section -->
    <div id="profile" class="">
        <div class="container my-5 py-5">
            <div class="col-lg">
                <div class="lc-block mb-3">
                    <div editable="rich">
                        <h2 class="fw-bold display-5 text-center inter-tight">
                            We aim to help each other
                        </h2>
                        <h2 class="fw-bold display-5 text-center dancing-script text-warning">
                            People Section Lorem Ipsum Dolor Sit Amet
                        </h2>
                        <p class="lead text-center inter-tight mt-3">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra.
                        </p>
                    </div>
                </div>
            </div>
            <div class="row">
                <ProfileCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Hastyana"
                    description="This is a people"
                    buttonText="See Profile"
                    @button-click="handleCardClick"
                />
                <ProfileCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Hastyana"
                    description="This is a people"
                    buttonText="See Profile"
                    @button-click="handleCardClick"
                />
                <ProfileCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Hastyana"
                    description="This is a people"
                    buttonText="See Profile"
                    @button-click="handleCardClick"
                />
                <ProfileCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Hastyana"
                    description="This is a people"
                    buttonText="See Profile"
                    @button-click="handleCardClick"
                />
            </div>
        </div>
    </div>

    <!-- Blog Section -->
    <div id="blog" class="">
        <div class="container my-5 py-5">
            <div class="col-lg">
                <div class="lc-block mb-3">
                    <div editable="rich">
                        <h2 class="fw-bold display-5 text-start inter-tight">
                            Whats happening
                        </h2>
                        <p class="lead text-start inter-tight mt-3">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra.
                        </p>
                    </div>
                </div>
            </div>
            <div class="row">
                <BlogCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Lorem Ipsum Article Blog 1 for Landing Page"
                    description="Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra."
                    buttonText="Read more"
                    @button-click="handleCardClick"
                />
                <BlogCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Lorem Ipsum Article Blog 1 for Landing Page"
                    description="Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra."
                    buttonText="Read more"
                    @button-click="handleCardClick"
                />
                <BlogCard
                    image="https://mdbootstrap.com/img/Photos/new-templates/animal-shelter/logo.png"
                    title="Lorem Ipsum Article Blog 1 for Landing Page"
                    description="Sed euismod, eros vitae convallis luctus, orci risus dictum quam, ac blandit dui orci non quam, nulla rutrum nisl augue, nec condimentum risus tristique ac. Integer bibendum ullamcorper pharetra."
                    buttonText="Read more"
                    @button-click="handleCardClick"
                />
            </div>
            <div class="lc-block d-grid gap-2 d-md-flex justify-content-md-end">
                <a class="btn btn-transparent px-4 me-md-2" href="#" role="button">See All</a>
            </div>
        </div>
    </div>

    <Footer />

</template>
  
  <script>
  export default {
    name: 'LandingPage',
    components: {
        BlogCard,
        BrandSlide,
        ProfileCard,
    },
    methods: {
        handleCardClick() {
        alert("Button clicked!");
        },
    },
  };
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  </style>
  