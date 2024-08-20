<script lang="ts">
  import NavBar from './NavBar.svelte';

  </script>

<NavBar/>
<main class="p-8 bg-base-content">
  <section class="text-center my-16 text-black">
      <h1 class="text-4xl font-bold mb-4">Welcome to Our Tutoring Services</h1>
      <p class="text-lg">We provide personalized tutoring to help you achieve your academic goals.</p>
  </section>

  <!-- Services Section -->
  <section class="my-16">
      <h2 class="text-3xl font-bold mb-8 text-center">Our Services</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="card bg-base-100 shadow-xl">
              <div class="card-body">
                  <h3 class="card-title">Math Tutoring</h3>
                  <p>Expert math tutoring for all levels, from elementary to college.</p>
              </div>
          </div>
          <div class="card bg-base-100 shadow-xl">
              <div class="card-body">
                  <h3 class="card-title">Science Tutoring</h3>
                  <p>Comprehensive science tutoring, including biology, chemistry, and physics.</p>
              </div>
          </div>
          <div class="card bg-base-100 shadow-xl">
              <div class="card-body">
                  <h3 class="card-title">Language Tutoring</h3>
                  <p>Improve your language skills with our experienced tutors.</p>
              </div>
          </div>
      </div>
  </section>

  <!-- Testimonials Section -->
  <section class="my-16">
      <h2 class="text-3xl font-bold mb-8 text-center">What Our Students Say</h2>
      <div class="carousel w-full">
          <div id="slide1" class="carousel-item relative w-full">
              <div class="card bg-base-100 shadow-xl mx-auto">
                  <div class="card-body">
                      <p>"The tutoring sessions have been incredibly helpful. My grades have improved significantly!"</p>
                      <h3 class="card-title">- Student A</h3>
                  </div>
              </div>
              <a href="#slide3" class="btn btn-circle absolute left-5 top-1/2 transform -translate-y-1/2">❮</a>
              <a href="#slide2" class="btn btn-circle absolute right-5 top-1/2 transform -translate-y-1/2">❯</a>
          </div>
          <div id="slide2" class="carousel-item relative w-full">
              <div class="card bg-base-100 shadow-xl mx-auto">
                  <div class="card-body">
                      <p>"The tutors are very knowledgeable and patient. I highly recommend their services."</p>
                      <h3 class="card-title">- Student B</h3>
                  </div>
              </div>
              <a href="#slide1" class="btn btn-circle absolute left-5 top-1/2 transform -translate-y-1/2">❮</a>
              <a href="#slide3" class="btn btn-circle absolute right-5 top-1/2 transform -translate-y-1/2">❯</a>
          </div>
          <div id="slide3" class="carousel-item relative w-full">
              <div class="card bg-base-100 shadow-xl mx-auto">
                  <div class="card-body">
                      <p>"Thanks to the tutoring, I feel much more confident in my studies."</p>
                      <h3 class="card-title">- Student C</h3>
                  </div>
              </div>
              <a href="#slide2" class="btn btn-circle absolute left-5 top-1/2 transform -translate-y-1/2">❮</a>
              <a href="#slide1" class="btn btn-circle absolute right-5 top-1/2 transform -translate-y-1/2">❯</a>
          </div>
      </div>
  </section>

  <!-- Contact Section -->
  <section class="my-16">
      <h2 class="text-3xl font-bold mb-8 text-center">Contact Us</h2>
      <form class="max-w-lg mx-auto bg-base-100 p-8 rounded-lg shadow-lg">
          <div class="form-control mb-4">
              <label class="label" for="name">
                  <span class="label-text">Name</span>
              </label>
              <input type="text" id="name" class="input input-bordered" placeholder="Your Name" />
          </div>
          <div class="form-control mb-4">
              <label class="label" for="email">
                  <span class="label-text">Email</span>
              </label>
              <input type="email" id="email" class="input input-bordered" placeholder="Your Email" />
          </div>
          <div class="form-control mb-4">
              <label class="label" for="message">
                  <span class="label-text">Message</span>
              </label>
              <textarea id="message" class="textarea textarea-bordered" placeholder="Your Message"></textarea>
          </div>
          <div class="form-control">
              <button type="submit" class="btn btn-primary">Send Message</button>
          </div>
      </form>
  </section>
</main>
