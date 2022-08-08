<template>
  <div class="container">
    <div class="top-story">
      <div class="col-left">
        <div class="main-top-story">
          <img src="https://i1-vnexpress.vnecdn.net/2022/08/03/topppppp-1659509955-4136-1659509958.jpg?w=680&h=408&q=100&dpr=1&fit=crop&s=TASyTJIBrZrxOffSAOD5kg" alt="">
          <div class="main-top-story-description">
            <h3>Hien trang 3 cao toc ket noi TPHCM</h3>
            <p>Các cao tốc từ TP HCM đi Long Thành - Dầu Giây, Trung Lương - Mỹ Thuận thường xuyên ùn tắc do nhỏ hẹp khiến các tài xế mệt mỏi, mong muốn sớm được mở rộng.</p>
          </div>
        </div>
        <div class="bottom-top-story">
          <ul>
            <li>
              <h4>Trực thăng quần thảo chiến đấu với đám cháy kho dầu Cuba</h4>
              <p>Giới chức Cuba triển khai nhiều lực lượng, trong đó có trực thăng, để đối phó vụ cháy lớn tại kho dầu Matanzas, tây bắc đất nước.</p>
            </li>
            <li>
              <h4>Chiến hạm Đài Loan bám sát tàu khu trục Trung Quốc</h4>
              <p>Lực lượng phòng vệ Đài Loan triển khai nhiều chiến hạm bám sát tàu khu trục, tàu hộ vệ Trung Quốc hiện diện ở phía đông và nam hòn đảo.</p>
            </li>
            <li class="item-gocnhin">
              <h5>Góc nhìn</h5>
              <h4>Cách tiêu tiền</h4>
              <p>Khi con tôi 6 tuổi, cháu được cung cấp 5 cái hũ, để bắt đầu quản lý tiền.</p>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-right">

      </div>
    </div>
    <hr>
  </div>
</template>

<script setup>

</script>

<style scoped>
.top-story {
  display: flex;
  margin: 20px 0;
}

.col-left {
  width: 780px;
  display: flex;
  flex-direction: column;
}

.main-top-story {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-right: 20px;
  background-color: #f7f7f7;

}

.main-top-story img {
  width: 520px;
  height: 312px;
  margin-right: 20px;
}

.main-top-story .main-top-story-description h3 {
  margin-bottom: 12px;
}

.main-top-story .main-top-story-description p {
  font-size: 14px;
}

.bottom-top-story {
  padding: 12px 0;
}

.bottom-top-story ul {
  list-style-type: none;
  display: flex;
  justify-content: space-around;
}

.bottom-top-story ul li {
  padding-right: 20px;
}

.bottom-top-story ul li h4 {
  margin-bottom: 12px;
}

.bottom-top-story ul li p {
  font-size: 14px;
}

.bottom-top-story .item-gocnhin {
  border-left: 1px solid #757577;
  padding-left: 20px;
}

.col-right {
  width: 320px;
  padding-left: 20px;
}
</style>