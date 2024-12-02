<template>
    <div>
      <nav class="navbar border p-3">
  <div class="container">
    <a class="navbar-brand " href="/">
      <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="#006fd6" class="bi bi-buildings" viewBox="0 0 16 16">
  <path d="M14.763.075A.5.5 0 0 1 15 .5v15a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5V14h-1v1.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V10a.5.5 0 0 1 .342-.474L6 7.64V4.5a.5.5 0 0 1 .276-.447l8-4a.5.5 0 0 1 .487.022M6 8.694 1 10.36V15h5zM7 15h2v-1.5a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 .5.5V15h2V1.309l-7 3.5z"/>
  <path d="M2 11h1v1H2zm2 0h1v1H4zm-2 2h1v1H2zm2 0h1v1H4zm4-4h1v1H8zm2 0h1v1h-1zm-2 2h1v1H8zm2 0h1v1h-1zm2-2h1v1h-1zm0 2h1v1h-1zM8 7h1v1H8zm2 0h1v1h-1zm2 0h1v1h-1zM8 5h1v1H8zm2 0h1v1h-1zm2 0h1v1h-1zm0-2h1v1h-1z"/>
</svg>
      <span class="wi">wiman-inn</span>
    </a>
   
    
  <input type="search" class="nav-link border-bottom w-50" placeholder="หาที่พัก" aria-label="Search" id="searchbar"><button class="btn btn-outline-primary border border-1 border-info ps-2 pe-2 rounded"> ค้นหา <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
  <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001q.044.06.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1 1 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0"/>
</svg></button>
    
    
    <a href="#" class="nav-link"><button class="btn btn-outline-primary border border-1 border-info ps-2 pe-2 rounded" data-bs-toggle="modal" data-bs-target="#LoginModal">เข้าสู่ระบบ</button></a>
    <a href="#" class="nav-link"><button class="btn btn-outline-primary border border-1 border-info ps-2 pe-2 rounded" data-bs-toggle="modal" data-bs-target="#RegisModal">สมัครสมาชิก</button></a>
    
  </div>

</nav>
<!--Modal login-->
<div
              class="modal fade"
              id="LoginModal"
              tabindex="-1"
              aria-labelledby="exampleModalLabel"
              aria-hidden="true"
            >
              <div class="modal-dialog">
                <div class="modal-content">
                  <div class="modal-header">
                    <h1 class="modal-title fs-5" id="exampleModalLabel">เข้าสู่ระบบ</h1>
                    <button
                      type="button"
                      class="btn-close"
                      data-bs-dismiss="modal"
                      aria-label="Close"
                    ></button>
                  </div>
                  <div class="modal-body">
                    กรอกข้อมูลเพื่อเข้าสู่ระบบ <br>
                    <label class="p-2" for="username">username</label><br>
                    <input type="text" class="form-control w-100" id="username" placeholder="โปรดกรอกชื่อผู้ใช้">
                    <label class="p-2" for="password" id="password">Password</label><br>
                    <input type="password" class="form-control w-100" id="password" placeholder="รหัสผ่าน"><br>
                    <button type="button" class="btn btn-success text-center" id="submit" @click="Alertwelcom"><a href="/ListProductVue" class="nav-link">Login</a></button>

                  </div>
                  <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                  </div>
                </div>
              </div>
            </div>
      <!--End Modal Login-->

      <!--Modal Register-->
<div
              class="modal fade"
              id="RegisModal"
              tabindex="-1"
              aria-labelledby="exampleModalLabel"
              aria-hidden="true"
            >
              <div class="modal-dialog">
                <div class="modal-content">
                  <div class="modal-header">
                    <h1 class="modal-title fs-5" id="exampleModalLabel">สมัครสมาชิก</h1>
                    <button
                      type="button"
                      class="btn-close"
                      data-bs-dismiss="modal"
                      aria-label="Close"
                    ></button>
                  </div>
                  <div class="modal-body">
                    กรอกข้อมูลเพื่อสมัครสมาชิก <br>
                    <label class="p-2" for="name">ชื่อ</label>
                    <input type="text" class="form-control w-100" id="name" placeholder="โปรดกรอกชื่อ ไม่ต้องมีคำนำหน้า">
                    <label class="p-2" for="lastname">นามสกุล</label>
                    <input type="text" class="form-control w-100" id="lastname" placeholder="โปรดกรอกนามสกุล">
                    <label class="p-2" for="teluser">เบอร์โทรศัพท์</label>
                    <input type="text" class="form-control w-100" id="teluser" placeholder="โปรดกรอกเบอร์โทร">

                    <label class="p-2" for="username">username</label>
                    <input type="text" class="form-control w-100" id="username" placeholder="ตั้งชื่อผู้ใช้">
                    <label class="p-2" for="password" id="password">Password</label><br>
                    <input type="password" class="form-control w-100" id="password" placeholder="รหัสผ่าน"><br>
                    <button type="button" class="btn btn-success text-center" id="submit" @click="showAlert"><a href="/" class="nav-link">sign in</a></button>
                    
                  </div>
                  <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                  </div>
                </div>
              </div>
            </div>
      <!--End Modal Register-->

    </div>
</template>
<script>



export default {
    name:'MenuVue',
    methods: { showAlert() { alert('สมัครข้อมูลสำเร็จ!');},
                Alertwelcom(){ alert('ยินดีต้อนรับ');}
                
  
  }
    
}

</script>
<style  scoped>
.navbar{
  background: none;
  font-family:'TH Sarabun NEW','Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: #006fd6;
  font-size: 150%;
  padding: 10px;
}
.navbar-link:hover{
  background-color: #006fd6;
  font-family:'TH Sarabun NEW','Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: #006fd6;
  font-size: 150%;
  padding: 10px;
  background-color: #006fd6;
}
.wi{
  
  font-family:'TH Sarabun NEW','Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: #006fd6;
  font-size: 30px;
  padding: 10px;
}
button{
  font-size: 20px;
}
</style>
    
      
