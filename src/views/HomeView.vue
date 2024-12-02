<template>
  <div class="home">
    <div id="carouselExampleCaptions" class="carousel slide">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="../assets/cover1.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h1>จองโรงแรม</h1>
        <p>จองโรงแรมหรู ใกล้สถาที่ท่องเที่ยว พร้อมบรรยากาศแสนพิเศษ</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/cover2.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h1>จองที่พัก</h1>
        <p>จองที่พักไว้พักผ่อนช่วงหยุดยาว หรือช่วงเทศกาล</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/cover3.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h1>ให้เราช่วยค้นหา</h1>
        <p>หาที่พักได้ตามที่คุณต้องการ ที่วิมาน.com</p>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
<div class="col-12 text-center">
<a href="/ListProductVue" ><button class="btn btn-outline-primary border border-1 border-info ps-2 pe-2 rounded my-2 mx-auto">เข้าสู่เว็บไซต์</button></a>
</div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  

  
                

  
}
</script>

<style scoped>
.carousel-inner img { width: 100%; /* ปรับให้รูปภาพเต็มความกว้างของ Carousel */ height: 500px; /* กำหนดความสูงของ Carousel */}
h1,p{
  font-family:'TH Sarabun NEW','Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-weight: bold;
  color: #ffffff;
  margin: 0%;
  background: rgba(65, 130, 252, 0.5)
}

p{font-size: 20px};
</style>
