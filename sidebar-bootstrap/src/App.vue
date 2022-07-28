<template>
<!-- flex-md-nowrap flex-wrap kalo sm flex row untuk md ke atas dan column untuk sm -->
  <div class="d-flex flex-md-nowrap flex-wrap flex-md-row flex-column">
    <!-- sticky agar tetap pada posisi ketika discroll -->
    <div class="border-bottom sticky-top col-lg-3 col-md-4 h-100 bg-white" style="max-height: 100vh; overflow: auto">
      <div class="p-3">
        <!-- navbar + -->
        <nav class="navbar navbar-expand-md bg-white">
          <div class="container-fluid">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <!-- flex-md-column -->
            <div class="collapse navbar-collapse flex-md-column" id="navbarTogglerDemo01">
              <a class="navbar-brand" href="#">Hidden brand</a>
              <!-- flex-md-column -->
              <ul class="navbar-nav me-auto mb-2 mb-lg-0 flex-md-column">
                <li class="nav-item">
                  <a class="nav-link active" aria-current="page" href="#">Home</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link disabled">Disabled</a>
                </li>
              </ul>
              <form class="d-flex" role="search">
                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-outline-success" type="submit">Search</button>
              </form>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <!-- content grow artinya mengisi tempat yang tersedia dari sidebar yang menggunakan col-md-4 dst -->
    <div class="flex-grow-1 position-relative z-index-">
      <div class="p-4">
        <div>
          <h3>
            Content Header
          </h3>
        </div>
        <div class="mb-3" v-for="i in 100" :key="i">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime autem cum nisi temporibus veniam? Maxime deleniti, iure vitae est, dolores perspiciatis distinctio voluptatibus autem quibusdam veritatis, blanditiis animi a eius.
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>