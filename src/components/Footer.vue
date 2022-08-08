<template>
    <div class="container">
        <footer class="footer-wrapper">
            <ul class="list-menu">
                <li>Trang chủ</li>
                <li>Video</li>
                <li>Podcasts</li>
                <li>Ảnh</li>
                <li>Infographics</li>
                <li><hr></li>
                <li>Mới nhất</li>
                <li>Xem nhiều</li>
                <li>Tin nóng</li>
            </ul>
            <ul class="list-menu">
                <li>Thời sự</li>
                <li>Góc nhìn</li>
                <li>Thế giới</li>
                <li>Kinh doanh</li>
                <li>Giải trí</li>
            </ul>
            <ul class="list-menu">
                <li>Thể thao</li>
                <li>Pháp luật</li>
                <li>Giáo dục</li>
                <li>Sức khỏe</li>
                <li>Đời sống</li>
                <li>Du lịch</li>
            </ul>
            <ul class="list-menu">
                <li>Khoa học</li>
                <li>Số hóa</li>
                <li>Xe</li>
                <li>Ý kiến</li>
                <li>Tâm sự</li>
                <li>Hài</li>
            </ul>
            <ul class="list-menu last-item">
                <li>Rao vặt</li>
                <li>Startup</li>
                <li>Mua ảnh VnExpress</li>
                <li>VHome</li>
                <li>eBox</li>
                <li>eWork</li>
            </ul>
            <div class="contact">
                <div class="contact-download-app">
                    <p>Tải ứng dụng</p>
                    <div class="download-app">
                        <a>VnExpress</a>
                        <a>International</a>
                    </div>
                </div>
                <div class="contact-box">
                    <p>Liên hệ</p>
                    <a href=""><span class="material-icons">email</span><span>Tòa soạn</span></a>
                    <a href="">Quảng cáo</a>
                    <a href=""><img src="https://s1.vnecdn.net/vnexpress/restruct/c/v1357/v2_2019/pc/images/graphics/logo_vlight.svg"><span>Hợp tác bản quyền</span></a>
                </div>
                <div class="hotline">
                    <p>Đường dây nóng</p>
                    <div class="left">
                        <strong>084.888.0123</strong>
                        <p>(Hà Nội)</p>
                    </div>
                    <div class="right">
                        <strong>084.888.0123</strong>
                        <p>(TP. Hồ Chí Minh)</p>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>

</script>

<style scoped>
ul {
    list-style-type: none;
}

.footer-wrapper {
    border-top: 5px solid #e5e5e5;
    border-bottom: 1px solid #e5e5e5;
    margin-top: 15px;
    padding: 20px 0;
    display: flex;
    width: 100%;
}

.list-menu {
    font-size: 14px;
    padding-right: 30px;
    width: 170px;
}

.list-menu li {
    margin-bottom: 15px;
}

.list-menu:first-child li{
    font-weight: 600;
}

.last-item {
    padding-left: 15px;
    border-right: 1px solid #e5e5e5;
    border-left: 1px solid #e5e5e5;
}

.contact {
    width: 250px;
    padding-left: 15px;
    font-size: 14px;
}

.contact .contact-download-app {
    margin-bottom: 8px;
}

.contact .contact-download-app .download-app {
    padding: 3px 0;
}

.contact .contact-download-app .download-app a{
    background-color: #f7f7f7;
    margin-right: 10px;
    border: 1px solid #e5e5e5;
    border-radius: 3px;
    width: 120px;
    font-size: 14px;
    text-align: center;
    padding: 2px 8px;
}

.contact p {
    color: #757575;
    margin-bottom: 6px;
}

.contact-box {
    border-bottom: 1px solid #e5e5e5;
    height: 150px;
}

.contact-box a{
    /* display: block; */
    width: 120px;
    float: left;
    line-height: 20px;
    margin: 0 10px 8px 0;
}


.hotline .left {
    float: left;
}

.hotline .right {
    float: right
}
</style>