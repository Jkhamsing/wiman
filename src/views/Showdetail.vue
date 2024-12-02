<template>
  <div>
    <div class="container">
      <h1>รายละเอียด</h1>

      <div class="row">
        <div class="col-6 p-3">
          <img src="../assets/A16_1.jpg" class="rounded float-end w-100" />
        </div>
        <div class="col-6 p-2 d-inline">
          <h1 class="bg-danger">
            <b>Notebook Asus TUF Gaming A16 FA617NSR-N3016W (Sandstorm)</b>
          </h1>

          <div class="col-12 p-3 text-start">
            <table>
              <tr>
                <th>แบรนด์</th>
                <td>ASUS</td>
              </tr>
              <tr>
                <th>โมเดล</th>
                <td>TUF Gaming A16 Advantage Edition (FA617NSR-N3016W)</td>
              </tr>
              <tr>
                <th>ตัวประมวลผล</th>
                <td>AMD Ryzen 7 7435HS Mobile Processor 3.1GHz (20MB Cache, up to 4.55GHz, 8 cores, 16 Threads)</td>
              </tr>
              <tr>
                <th>กราฟฟิค</th>
                <td>AMD Radeon RX 7600S (8GB GDDR6), up to 95W(SmartShift)</td>
              </tr>
              <tr>
                <th>จอภาพ</th>
                <td>16.0", 1920x1200 (WUXGA) 16:10, IPS, 165Hz, anti-glare, 100% sRGB, 75.35% Adobe, 7ms, FreeSync Premium</td>
              </tr>
              <tr>
                <th>ความจำสำรอง (RAM)</th>
                <td>16GB DDR5 4800MHz (Max Memory 32GB)</td>
              </tr>
              <tr>
                <th>ความจุ</th>
                <td>512GB PCIe 4.0 NVMe M.2 SSD</td>
              </tr>
              <tr>
                <th>พอร์ต</th>
                <td>
                  1x HDMI 2.1 FRL
                  <br />1x USB 3.2 Gen 2 Type-C
                  <br />2x USB 3.2 Gen 1 Type-A
                  <br />2x USB 3.2 Gen 1 Type-C support DisplayPort / power delivery
                </td>
              </tr>
              <tr>
                <th>แบตเตอร์รี่</th>
                <td>90WHrs, 4S1P, 4-cell Li-ion</td>
              </tr>
              <tr>
                <th>ระบบปฎิบัติการ</th>
                <td>Windows 11 Home</td>
              </tr>
            </table>

            <button
              type="button"
              class="btn btn-danger my-3 w-100"
              data-bs-toggle="modal"
              data-bs-target="#exampleModal"
            >สั่งซื้อ</button>

            <div
              class="modal fade"
              id="exampleModal"
              tabindex="-1"
              aria-labelledby="exampleModalLabel"
              aria-hidden="true"
            >
              <div class="modal-dialog">
                <div class="modal-content">
                  <div class="modal-header">
                    <h1 class="modal-title fs-5" id="exampleModalLabel">ยืนยันการซื้อ</h1>
                    <button
                      type="button"
                      class="btn-close"
                      data-bs-dismiss="modal"
                      aria-label="Close"
                    ></button>
                  </div>
                  <div class="modal-body">
                    โปรดแสกน QR Code เพื่อติดต่อเจ้าหน้าที่
                    <img src="../assets/qr.jpg" alt />
                  </div>
                  <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ShowVue"
};
</script>
<style>
.topic {
  font-size: 20px;
  font-weight: bold;
  text-align: left;
}

tr,
th {
  border: 2px solid;
  padding: 5px;
  width: 20%;
}
td {
  border: 2px solid;
  padding: 5px;
}
</style>