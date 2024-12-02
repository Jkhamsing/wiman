<template>
    <div>
        <div class="container">
          <div class="row">
            <!--filters-->
            <div class="col-2 my-2 py-4 bg-info-subtle rounded">
              <h5>ค้นหาตามตัวกรอง</h5>
              <p><b>คะแนน <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-star-fill" viewBox="0 0 16 16">
  <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.282.95l-3.522 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
</svg></b></p>
              <form> 
                <div class="form-check"> <input class="form-check-input" type="checkbox" value="5star" id="rate"> 
              <label class="form-check-label" for="defaultCheck1">5 ดาว </label> 
              </div> 
              <div class="form-check"> <input class="form-check-input" type="checkbox" value="4star" id="rate" > 
              <label class="form-check-label" for="defaultCheck2">4 ดาว</label> 
              </div>
              <div class="form-check"> <input class="form-check-input" type="checkbox" value="3star" id="rate"> 
              <label class="form-check-label" for="defaultCheck1">3 ดาว </label> 
              </div> 
              <div class="form-check"> <input class="form-check-input" type="checkbox" value="2star" id="rate" > 
              <label class="form-check-label" for="defaultCheck2">2 ดาว</label> 
              </div> 
            
              </form>
              <p><b>ประเภท <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-houses-fill" viewBox="0 0 16 16">
  <path d="M7.207 1a1 1 0 0 0-1.414 0L.146 6.646a.5.5 0 0 0 .708.708L1 7.207V12.5A1.5 1.5 0 0 0 2.5 14h.55a2.5 2.5 0 0 1-.05-.5V9.415a1.5 1.5 0 0 1-.56-2.475l5.353-5.354z"/>
  <path d="M8.793 2a1 1 0 0 1 1.414 0L12 3.793V2.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5v3.293l1.854 1.853a.5.5 0 0 1-.708.708L15 8.207V13.5a1.5 1.5 0 0 1-1.5 1.5h-8A1.5 1.5 0 0 1 4 13.5V8.207l-.146.147a.5.5 0 1 1-.708-.708z"/>
</svg></b></p>
              <form> 
                <div class="form-check"> <input class="form-check-input" type="checkbox" value="hotel" id="type"> 
              <label class="form-check-label" for="defaultCheck1">โรงแรม </label> 
              </div> 
              <div class="form-check"> <input class="form-check-input" type="checkbox" value="homstay" id="type" > 
              <label class="form-check-label" for="defaultCheck2">โฮมสเตย์</label> 
              </div>
              <div class="form-check"> <input class="form-check-input" type="checkbox" value="resident" id="type"> 
              <label class="form-check-label" for="defaultCheck1">บ้านพัก</label> 
              </div> 
              </form>
              <button class="btn btn-info my-2 w-100" id="sentfilter" @click="findfilter">ค้นหา</button>
            </div>

      <!--End Filter-->
            <div class="col-10 my-2">
              <h4>ที่พัก</h4>
      
      <!--Start list-->
              <div class="row p-2 mx-1 border rounded" id="aa" v-if="isDivVisible">
                <div class="col"><img src="../assets/ho2.jpg" class="imgshow"></div>
                <div class="col">
                  <h3>เอเอ โฮเทล พัทยา</h3>
                  <label for="rate" id="rate4"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-star-fill" viewBox="0 0 16 16">
  <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.282.95l-3.522 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
</svg>  4 ดาว</label><br>
                  <label for="type" id="hotel" class=" my-1 px-2 bg-info rounded">โรงแรม</label>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
  <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10m0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6"/>
</svg> 182-182/2 ซอย 13 ถ.หาดพัทยา ชลบุรี, 20260 พัทยากลาง, บางละมุง, จังหวัดชลบุรี, 20260</p>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-telephone-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z"/>
</svg> 081 - 2345678</p>

                  <h5 class="mt-4"><b>ข้อมูลห้องพัก</b></h5>
                  <table>
                    <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-aspect-ratio" viewBox="0 0 16 16">
  <path d="M0 3.5A1.5 1.5 0 0 1 1.5 2h13A1.5 1.5 0 0 1 16 3.5v9a1.5 1.5 0 0 1-1.5 1.5h-13A1.5 1.5 0 0 1 0 12.5zM1.5 3a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h13a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5z"/>
  <path d="M2 4.5a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 0 1H3v2.5a.5.5 0 0 1-1 0zm12 7a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1 0-1H13V8.5a.5.5 0 0 1 1 0z"/>
</svg></td>
                    <td>3 ตร.เมตร</td>
                    <td><img src="../assets/bed.svg" width="32" height="32" color="#2c3e50"></td>
                    <td>เตียงคู่</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-box-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M15.528 2.973a.75.75 0 0 1 .472.696v8.662a.75.75 0 0 1-.472.696l-7.25 2.9a.75.75 0 0 1-.557 0l-7.25-2.9A.75.75 0 0 1 0 12.331V3.669a.75.75 0 0 1 .471-.696L7.443.184l.004-.001.274-.11a.75.75 0 0 1 .558 0l.274.11.004.001zm-1.374.527L8 5.962 1.846 3.5 1 3.839v.4l6.5 2.6v7.922l.5.2.5-.2V6.84l6.5-2.6v-.4l-.846-.339Z"/>
</svg></td>
                    <td>มีเฟอร์นิเจอร์</td>
                  </tr>
                  <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-wifi" viewBox="0 0 16 16">
  <path d="M15.384 6.115a.485.485 0 0 0-.047-.736A12.44 12.44 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.52.52 0 0 0 .668.05A11.45 11.45 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049"/>
  <path d="M13.229 8.271a.482.482 0 0 0-.063-.745A9.46 9.46 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065m-2.183 2.183c.226-.226.185-.605-.1-.75A6.5 6.5 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.5 5.5 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091zM9.06 12.44c.196-.196.198-.52-.04-.66A2 2 0 0 0 8 11.5a2 2 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z"/>
</svg></td>
                    <td>Wi-Fi</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-c-square-fill" viewBox="0 0 16 16">
  <path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zm6.146 4.992c-1.212 0-1.927.92-1.927 2.502v1.06c0 1.571.703 2.462 1.927 2.462.979 0 1.641-.586 1.729-1.418h1.295v.093c-.1 1.448-1.354 2.467-3.03 2.467-2.091 0-3.269-1.336-3.269-3.603V7.482c0-2.261 1.201-3.638 3.27-3.638 1.681 0 2.935 1.054 3.029 2.572v.088H9.875c-.088-.879-.768-1.512-1.729-1.512"/>
</svg></td>
                    <td>ส่วนกลาง :สระว่ายน้ำ</td>
                  </tr>
                  </table>
                  <p class="my-3 text-primary fs-2"><b>ราคา 599บาท /คืน</b></p>
                  <button class="btn btn-info w-100" data-bs-toggle="modal" data-bs-target="#d001">รายละเอียด</button>
  

   
                </div>
              </div>
      <!--End list-->

      <!--Start list-->
      <div class="row p-2 mx-1 border rounded" >
                <div class="col"><img src="../assets/hs1.jpg" class="imgshow"></div>
                <div class="col">
                  <h3>ต้นหว้ารีสอร์ท</h3>
                  <label for="rate" id="rate"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-star-fill" viewBox="0 0 16 16">
  <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.282.95l-3.522 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
</svg>  5 ดาว</label><br>
                  <label for="type" id="type" class=" my-1 px-2 bg-info rounded">โฮมสเตย์</label>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
  <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10m0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6"/>
</svg> 55 Chaloem Burapha Chonlathit Road, หาดเจ้าหลาว, จันทบุรี, ไทย, 22120</p>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-telephone-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z"/>
</svg> 098 - 7654321</p>

                  <h5 class="mt-4"><b>ข้อมูลห้องพัก</b></h5>
                  <table>
                    <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-aspect-ratio" viewBox="0 0 16 16">
  <path d="M0 3.5A1.5 1.5 0 0 1 1.5 2h13A1.5 1.5 0 0 1 16 3.5v9a1.5 1.5 0 0 1-1.5 1.5h-13A1.5 1.5 0 0 1 0 12.5zM1.5 3a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h13a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5z"/>
  <path d="M2 4.5a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 0 1H3v2.5a.5.5 0 0 1-1 0zm12 7a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1 0-1H13V8.5a.5.5 0 0 1 1 0z"/>
</svg></td>
                    <td>4 ตร.เมตร</td>
                    <td><img src="../assets/bed.svg" width="32" height="32" color="#2c3e50"></td>
                    <td>เตียงคู่</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-box-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M15.528 2.973a.75.75 0 0 1 .472.696v8.662a.75.75 0 0 1-.472.696l-7.25 2.9a.75.75 0 0 1-.557 0l-7.25-2.9A.75.75 0 0 1 0 12.331V3.669a.75.75 0 0 1 .471-.696L7.443.184l.004-.001.274-.11a.75.75 0 0 1 .558 0l.274.11.004.001zm-1.374.527L8 5.962 1.846 3.5 1 3.839v.4l6.5 2.6v7.922l.5.2.5-.2V6.84l6.5-2.6v-.4l-.846-.339Z"/>
</svg></td>
                    <td>มีเฟอร์นิเจอร์</td>
                  </tr>
                  <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-wifi" viewBox="0 0 16 16">
  <path d="M15.384 6.115a.485.485 0 0 0-.047-.736A12.44 12.44 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.52.52 0 0 0 .668.05A11.45 11.45 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049"/>
  <path d="M13.229 8.271a.482.482 0 0 0-.063-.745A9.46 9.46 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065m-2.183 2.183c.226-.226.185-.605-.1-.75A6.5 6.5 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.5 5.5 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091zM9.06 12.44c.196-.196.198-.52-.04-.66A2 2 0 0 0 8 11.5a2 2 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z"/>
</svg></td>
                    <td>Wi-Fi</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-c-square-fill" viewBox="0 0 16 16">
  <path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zm6.146 4.992c-1.212 0-1.927.92-1.927 2.502v1.06c0 1.571.703 2.462 1.927 2.462.979 0 1.641-.586 1.729-1.418h1.295v.093c-.1 1.448-1.354 2.467-3.03 2.467-2.091 0-3.269-1.336-3.269-3.603V7.482c0-2.261 1.201-3.638 3.27-3.638 1.681 0 2.935 1.054 3.029 2.572v.088H9.875c-.088-.879-.768-1.512-1.729-1.512"/>
</svg></td>
                    <td>สระว่ายน้ำส่วนตัว</td>
                  </tr>
                  </table>
                  <p class="my-3 text-primary fs-2"><b>ราคา 635บาท /คืน</b></p>
                  <button class="btn btn-info w-100" data-bs-toggle="modal" data-bs-target="#d002">รายละเอียด</button>
  

   
                </div>
              </div>
      <!--End list-->

            <!--Start list-->
            <div class="row p-2 mx-1 border rounded">
                <div class="col"><img src="../assets/re3.jpg" class="imgshow"></div>
                <div class="col">
                  <h3>บ้านพักบางแสน บ้านชนัญญา BaanChananya</h3>
                  <label for="rate" id="rate"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-star-fill" viewBox="0 0 16 16">
  <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.282.95l-3.522 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
</svg>  5 ดาว</label><br>
                  <label for="type" id="type" class=" my-1 px-2 bg-info rounded">บ้านพัก</label>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
  <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10m0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6"/>
</svg> 102/7 หาดวอนนภา ถนน บางแสนล่าง ชลบุรี</p>
                  <p class="my-2 ">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-telephone-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z"/>
</svg> 098 - 1234567</p>

                  <h5 class="mt-4"><b>ข้อมูลห้องพัก</b></h5>
                  <table>
                    <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-aspect-ratio" viewBox="0 0 16 16">
  <path d="M0 3.5A1.5 1.5 0 0 1 1.5 2h13A1.5 1.5 0 0 1 16 3.5v9a1.5 1.5 0 0 1-1.5 1.5h-13A1.5 1.5 0 0 1 0 12.5zM1.5 3a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h13a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5z"/>
  <path d="M2 4.5a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 0 1H3v2.5a.5.5 0 0 1-1 0zm12 7a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1 0-1H13V8.5a.5.5 0 0 1 1 0z"/>
</svg></td>
                    <td>6 ตร.เมตร 2 ชั้น</td>
                    <td><img src="../assets/bed.svg" width="32" height="32" color="#2c3e50"></td>
                    <td>เตียงคู่ x 2</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-box-fill" viewBox="0 0 16 16">
  <path fill-rule="evenodd" d="M15.528 2.973a.75.75 0 0 1 .472.696v8.662a.75.75 0 0 1-.472.696l-7.25 2.9a.75.75 0 0 1-.557 0l-7.25-2.9A.75.75 0 0 1 0 12.331V3.669a.75.75 0 0 1 .471-.696L7.443.184l.004-.001.274-.11a.75.75 0 0 1 .558 0l.274.11.004.001zm-1.374.527L8 5.962 1.846 3.5 1 3.839v.4l6.5 2.6v7.922l.5.2.5-.2V6.84l6.5-2.6v-.4l-.846-.339Z"/>
</svg></td>
                    <td>มีเฟอร์นิเจอร์</td>
                  </tr>
                  <tr>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-wifi" viewBox="0 0 16 16">
  <path d="M15.384 6.115a.485.485 0 0 0-.047-.736A12.44 12.44 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.52.52 0 0 0 .668.05A11.45 11.45 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049"/>
  <path d="M13.229 8.271a.482.482 0 0 0-.063-.745A9.46 9.46 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065m-2.183 2.183c.226-.226.185-.605-.1-.75A6.5 6.5 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.5 5.5 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091zM9.06 12.44c.196-.196.198-.52-.04-.66A2 2 0 0 0 8 11.5a2 2 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z"/>
</svg></td>
                    <td>Wi-Fi</td>
                    <td><svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-c-square-fill" viewBox="0 0 16 16">
  <path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zm6.146 4.992c-1.212 0-1.927.92-1.927 2.502v1.06c0 1.571.703 2.462 1.927 2.462.979 0 1.641-.586 1.729-1.418h1.295v.093c-.1 1.448-1.354 2.467-3.03 2.467-2.091 0-3.269-1.336-3.269-3.603V7.482c0-2.261 1.201-3.638 3.27-3.638 1.681 0 2.935 1.054 3.029 2.572v.088H9.875c-.088-.879-.768-1.512-1.729-1.512"/>
</svg></td>
                    <td>ติดหาดวอนนภา</td>
                  </tr>
                  </table>
                  <p class="my-3 text-primary fs-2"><b>ราคา 800บาท /คืน</b></p>
                  <button class="btn btn-info w-100" data-bs-toggle="modal" data-bs-target="#d003">รายละเอียด</button>
  

   
                </div>
              </div>
      <!--End list-->
            </div>
            <!--here-->
<!--Modal-->
<div class="modal fade" id="d001" tabindex="-1" aria-labelledby="DetailModal" aria-hidden="true">
  <div class="modal-dialog  modal-fullscreen">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">รายละเอียด</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <div class="row border">
        <div class="col-6 border">
          <div class="scroll-container">
            <img src="../assets/ho1.jpg" alt="">
            <img src="../assets/ho2.jpg" alt="">
            <img src="../assets/ho3.jpg" alt="">
            <img src="../assets/ho4.jpg" alt="">
            <img src="../assets/ho5.jpg" alt="">
          </div>
          </div>
          <div class="col-6 border">
            <h3><b>โรงแรมเอเอ พัทยา (A.A. Pattaya Hotel)</b></h3>
            <p>สัมผัสประสบการณ์ชีวิตยามค่ำคืนที่มีชีวิตชีวา ศูนย์การค้า และทิวทัศน์ชายหาดที่สวยงามของพัทยาในฐานะนักเดินทางคนเดียวที่โรงแรมเอ.เอ. พัทยา เพลิดเพลินกับการแช่ตัวในสระว่ายน้ำเพื่อความสดชื่น ค็อกเทลที่บาร์ และเอร็ดอร่อยที่ร้านกาแฟ ห้องพักที่มีอุปกรณ์ครบครัน ให้บริการเครื่องปรับอากาศ Wi-Fi ฟรี และฝักบัวอันสดชื่น ใกล้หาดพัทยา เซ็นทรัลเฟสติวัลพัทยาบีช และป้ายเมืองพัทยา - จุดชมวิว เพื่อการเที่ยวชมที่ง่ายดาย ชื่นชมการบริการของแผนกต้อนรับที่ยอดเยี่ยมและทำเลที่ตั้งของโรงแรมใกล้ถนนคนเดิน ถนนเลียบชายหาด และอ่าวพัทยา จองเลย รับประสบการณ์สุดพิเศษ!</p>
            <h4>กรอกรายระเอียดเพื่อทำการจองที่พัก</h4>
            <label for="amountrent">จำนวนห้องที่จอง</label>
            <input class="form-control w-25" type="number" id="amountrent">
            <label for="checkin">ต้องการเข้าพักวันที่</label>
            <input class="form-control" type="date">
            <label for="checkout">ถึงวันที่</label>
            <input class="form-control" type="date">
            <label for="name">ชื่อผู้เข้าพัก</label>
            <input class="form-control" type="text"><label for="lastname">นามสกุล</label>
            <input class="form-control" type="text">
            <label for="teluser">เบอร์โทรศัพท์</label>
            <input class="form-control" type="text">
            <label for="formFile" class="form-label">แนบสลิปการโอน</label>
            <input class="form-control" type="file" id="formFile">
            
          </div>
        </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary" id="booking" @click="booking">จองเลย</button>
      </div>
    </div>
  </div>
</div>
              </div>
    <!--EndModal-->
     <!--Modal-->
<div class="modal fade" id="d002" tabindex="-1" aria-labelledby="DetailModal" aria-hidden="true">
  <div class="modal-dialog  modal-fullscreen">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">รายละเอียด</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <div class="row border">
        <div class="col-6 border">
          <div class="scroll-container">
            <img src="../assets/hs1.jpg" alt="">
            <img src="../assets/hs2.jpg" alt="">
            <img src="../assets/hs3.jpg" alt="">
            <img src="../assets/hs4.jpg" alt="">
            <img src="../assets/hs5.jpg" alt="">
          </div>
          </div>
          <div class="col-6 border">
            <h3><b>ต้นหว้ารีสอร์ท</b></h3>
            <p>ที่พักตั้งอยู่ในย่านหาดเจ้าหลาวของจันทบุรี ผู้เข้าพักจึงได้อยู่ใกล้สถานที่ท่องเที่ยวน่าสนใจและร้านอาหารอร่อยๆ</p>
            <h4>กรอกรายระเอียดเพื่อทำการจองที่พัก</h4>
            <label for="amountrent">จำนวนห้องที่จอง</label>
            <input class="form-control w-25" type="number" id="amountrent">
            <label for="checkin">ต้องการเข้าพักวันที่</label>
            <input class="form-control" type="date">
            <label for="checkout">ถึงวันที่</label>
            <input class="form-control" type="date">
            <label for="name">ชื่อผู้เข้าพัก</label>
            <input class="form-control" type="text"><label for="lastname">นามสกุล</label>
            <input class="form-control" type="text">
            <label for="teluser">เบอร์โทรศัพท์</label>
            <input class="form-control" type="text">
            <label for="formFile" class="form-label">แนบสลิปการโอน</label>
            <input class="form-control" type="file" id="formFile">
            
          </div>
        </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary" id="booking" @click="booking">จองเลย</button>
      </div>
    </div>
  </div>
</div>
              </div>
    <!--EndModal-->
 <!--Modal-->
 <div class="modal fade" id="d003" tabindex="-1" aria-labelledby="DetailModal" aria-hidden="true">
  <div class="modal-dialog  modal-fullscreen">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">รายละเอียด</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <div class="row border">
        <div class="col-6 border">
          <div class="scroll-container">
            <img src="../assets/re1.jpg" alt="">
            <img src="../assets/re2.jpg" alt="">
            <img src="../assets/re3.jpg" alt="">
            <img src="../assets/re4.jpg" alt="">
            <img src="../assets/re5.jpg" alt="">
          </div>
          </div>
          <div class="col-6 border">
            <h3><b>บ้านพักบางแสน บ้านชนัญญา BaanChananya</b></h3>
            <p>บ้านพักบางแสน บ้านชนัญญา BaanChananya อยู่ใน Ban Thai Don (1) ห่างจากหาดวอนนภา 100 ม. และให้บริการห้องนั่งเล่นพร้อมโทรทัศน์จอแบน บ้านพักนี้มอบบริการที่จอดรถส่วนตัวฟรี เลานจ์ส่วนกลาง และอินเทอร์เน็ตไร้สาย (WiFi) ฟรี บ้านพักติดตั้งเครื่องปรับอากาศนี้มี 4 ห้องนอนและ 2 ห้องน้ำพร้อมฝักบัวและอ่างอาบน้ำ บ้านพักบางแสน บ้านชนัญญา BaanChananya มีลานระเบียงให้ผู้เข้าพักใช้บริการ หาดบางแสน อยู่ห่างจากที่พักนี้ 1.1 กม. ส่วนคริสตัล เบย์ กอล์ฟคลับ อยู่ห่างจากที่พัก 10 กม. สนามบินที่ใกล้ที่สุดคือสนามบินนานาชาติสุวรรณภูมิ ซึ่งห่างจากบ้านพักบางแสน บ้านชนัญญา BaanChananya 68 กม.</p>
            <h4>กรอกรายระเอียดเพื่อทำการจองที่พัก</h4>
            <label for="amountrent">จำนวนห้องที่จอง</label>
            <input class="form-control w-25" type="number" id="amountrent">
            <label for="checkin">ต้องการเข้าพักวันที่</label>
            <input class="form-control" type="date">
            <label for="checkout">ถึงวันที่</label>
            <input class="form-control" type="date">
            <label for="name">ชื่อผู้เข้าพัก</label>
            <input class="form-control" type="text"><label for="lastname">นามสกุล</label>
            <input class="form-control" type="text">
            <label for="teluser">เบอร์โทรศัพท์</label>
            <input class="form-control" type="text">
            <label for="formFile" class="form-label">แนบสลิปการโอน</label>
            <input class="form-control" type="file" id="formFile">
            
          </div>
        </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary" id="booking" @click="booking">จองเลย</button>
      </div>
    </div>
  </div>
</div>
              </div>
    <!--EndModal-->
     

          </div>



        </div> 
    </div>
</template>
<script>
export default {
    name:'ListProductVue',
    data() { return { isDivVisible: true }
                            
  
           }, 
    methods: { findfilter() { this.isDivVisible = !this.isDivVisible },
    booking(){ alert('จองสำเร็จแล้ว');}
  
             }
}

</script>
<style>
    td { 
      padding: 3px;
    }
    .imgshow{
      width: 100%;
    }
    
    div.scroll-container {
  background-color: #333;
  overflow: auto;
  white-space: nowrap;
  padding: 2px;
}

div.scroll-container img {
  padding: 2px;
  width: 100%;
}

   
</style>