<template>
  <div class="box-category">
    <div class="box-catergory-featured">
        <ul>
            <li><h2>Thể thao</h2></li>
            <li>Bóng đá</li>
            <li>Tennis</li>
            <li>Marathon</li>
            <li>Lịch thi đấu</li>
        </ul>
    </div>
    <div class="box-category-news">
        <div class="top-news">
            <div class="news-item main-article">
                <img src="https://i1-thethao.vnecdn.net/2022/08/07/058991750a-1659860197-8160-1659860204.jpg?w=380&h=228&q=100&dpr=1&fit=crop&s=bKpXCNsFdkDgJKuwx6HW6w" alt="" width="225" height="135">
                <div class="description">
                    <h3>Ten Hag chấp nhận chiến thắng 'xấu xí'</h3>
                    <p>ANHTrước trận mở màn Ngoại hạng Anh gặp Brighton hôm nay, HLV Erik ten Hag muốn Man Utd đá đẹp mắt nhưng vẫn có thể thắng "xấu xí" khi cần ...</p>
                </div>
            </div>
            <div class="news-item right-article">
                <div class="description">
                    <h3>Kyrgios đoạt danh hiệu đầu tiên sau ba năm</h3>
                    <p>MỸNick Kyrgios đoạt danh hiệu ATP thứ bảy trong sự nghiệp khi hạ Yoshihito Nishioka 6-4, 6-3 ở giải Citi Open ngày 7/8. </p>
                </div>
            </div>
        </div>
        <ul class="bottom-news">
            <li>Những VĐV đầu tiên đăng ký Aquaman Vietnam</li>
            <li>Ten Hag: 'Dẫn dắt Man Utd thật khó khăn'</li>
            <li>Lewandowski ghi bàn đầu tiên cho Barca</li>
        </ul>
    </div>
  </div>
</template>

<script setup>
import ItemNews from './ItemNews.vue'
</script>

<style scoped>
.box-category {
    margin-bottom: 12px;
    border-bottom: 1px solid #e5e5e5;
}

.box-catergory-featured ul{
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    list-style: none;
}

.box-catergory-featured ul li {
    margin-right: 20px;
    font-size: 13px;
}

.box-catergory-featured ul li h2 {
    text-decoration: underline;
    text-decoration-color: brown;
}

.box-category-news {
    display: flex;
    flex-direction: column;
}

.box-category-news .top-news{
    display: flex;
    font-size: 14px;
    padding-bottom: 12px;
}

.box-category-news .news-item .description{
    padding: 0 20px;
}

.box-category-news .news-item .description h3 {
    margin-bottom: 6px;
}

.box-category-news .main-article {
    display: flex;
    border-right: 1px solid #e5e5e5;
    width: 67.648%;
}

.box-category-news .right-article {
    width: 32.352%;
}

.box-category-news .bottom-news {
    display: flex;
    justify-content: space-between;
    font-size: 14px;
    font-weight: 600;
    border-top: 1px solid #e5e5e5;
    padding: 10px 0 0 15px;
    margin-bottom: 10px;
}

.box-category-news .bottom-news li {
    max-width: 200px;
}
</style>