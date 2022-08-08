<template>
  <div class="container">
    <section class="main-section">
        <div class="col-left">
            <ul>
                <li v-for="(itemNews, index) in itemsNews" :key="index">
                    <ItemNews :title="itemNews.title" :img="itemNews.img" :description="itemNews.description"/>
                </li>
            </ul>
        </div>
        <div class="col-right">
            <ul>
                <li>
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                    <BoxCategory />
                </li>
            </ul>
        </div>
    </section>
  </div>
</template>

<script setup>
import ItemNews from '../components/ItemNews.vue'
import BoxCategory from '../components/BoxCategory.vue'

const itemsNews = [
    {
        title: 'Những pha chạm bóng của Quang Hải ở trận hòa Dijon',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/07/quanghai58841658718441-1659836-2650-6665-1659836317.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=wMJ8aQsyWy0sc7uJG3SS3w',
        description: 'PHÁPTiền vệ Nguyễn Quang Hải đá chính, tạo ra một số pha bóng ấn tượng trước khi rời sân phút 68 trong trận hòa 0-0 giữa Pau FC và Dijon ở vòng 2 Ligue 2.'
    },
    {
        title: 'Ba lý do quận, huyện TP HCM chậm chi tiền hỗ trợ nhà trọ',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/06/IMG-1886-JPG-5952-1659789119.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=P9QvfDS7MyA6soo7ZFTa8w',
        description: 'Hồ sơ từ doanh nghiệp nộp về quận bị tắc, chờ xác nhận đủ ba tháng, cán bộ sợ sai bị kỷ luật là những nguyên nhân khiến gói hỗ trợ nhà trọ ở TP HCM chậm trễ.'
    },
    {
        title: 'Chi hàng trăm triệu đồng kéo dài chân để đổi vận số',
        img: 'https://i1-suckhoe.vnecdn.net/2022/08/04/12-1659604410-1659604490-5146-1659604647.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=nqpQa6ux_VVg1PugP-q-Ng',
        description: 'HÀ NỘINam 32 tuổi cao 1,6 m, quyết định chi 350 triệu đồng để phẫu thuật kéo chân dài thêm 10 cm, với mong muốn thay đổi vận mệnh.'
    },
    {
        title: 'Hàng nghìn khán giả dầm mưa cổ vũ The Moffatts, 911, A1, Blue',
        img: 'https://i1-giaitri.vnecdn.net/2022/08/07/hay-fest-kha-n-gia-6463-165980-6282-5628-1659809516.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=KAyqqSkj704221AsFLsomQ',
        description: 'HÀ NỘIKhán giả đứng dưới mưa năm tiếng, cổ vũ nhóm nhạc đình đám - The Moffatts, 911, A1, Blue - ở show tối 6/8. '
    },
    {
        title: 'Lãi tiền tỷ từ trồng rong nho',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/06/rongnho-2-1659797667-5094-1659797993.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=65Y0tsGvSvraZzzM0O4upQ',
        description: 'KHÁNH HÒAThua lỗ đến mức từng cầm cố nhà cửa, anh Nguyễn Quang Duy, 42 tuổi, vẫn kiên trì theo đuổi, đến nay mỗi tháng thu về 6 tỷ đồng từ rong nho, lãi gần hai tỷ'
    },
    {
        title: 'Máy ép nước cốt dừa tự chế của nhóm thanh niên',
        img: '',
        description: 'TP HCMChung đam mê chế tạo máy, nhóm bạn gồm 4 thành viên cùng nhau chế tạo máy ép nước cốt dừa với mục đích giúp người thân trong việc làm bánh.'
    },
    {
        title: 'Ngày thứ 164 chiến sự: Nhà máy hạt nhân Ukraine thiệt hại nặng',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/07/32933nf-highres-1659585396-566-9108-9911-1659806766.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=E-XDPf7l7IJjnAn6eV5-hw',
        description: 'Ukraine và Nga đổ lỗi qua lại về những vụ nổ gây thiệt hại nặng trong nhà máy điện hạt nhân Zaporizhzhia phía nam Ukraine. '
    },
    {
        title: 'Quang Hải đá chính trong trận hoà của Pau',
        img: 'https://i1-thethao.vnecdn.net/2022/08/07/quang-ha-i-jpeg-1659813359-3969-1659813397.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=ZlHYd835L8YwOSIAsMj0BQ',
        description: 'PHÁPTiền vệ Nguyễn Quang Hải lần đầu đá chính, chơi 68 phút khi Pau hoà đội khách Dijon 0-0 ở vòng hai Ligue 2 tối 6/8.'
    },
    {
        title: 'Chủ nhà hàng trong vụ "8 sinh viên bị ngộ độc" khai gì?',
        img: '',
        description: 'TP HCMNgười đại diện pháp luật của nhà hàng - nơi 8 sinh viên nhậu rồi bị ngộ độc khiến 2 người tử vong, cho biết 6 nạn nhân là nhân viên phục vụ tại quán'
    },
    {
        title: 'Chelsea thắng nhờ phạt đền',
        img: 'https://i1-thethao.vnecdn.net/2022/08/07/a-2117-1659811534.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=exGv9l7c88DqSWULa6cj6Q',
        description: 'ANHTiền vệ Jorginho ghi bàn duy nhất từ chấm 11m, giúp Chelsea thắng 1-0 trên sân Everton ở vòng 1 Ngoại hạng Anh, tối 6/8. '
    },
    {
        title: 'Lao động xuất khẩu khó kiếm việc khi về nước',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/06/A1-1659802641-8463-1659802871.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=es7AmN83W5IvuMU8xvntmA',
        description: 'Buộc phải về nước do dịch, Nguyệt thất nghiệp nhiều tháng vì làm công nhân tại Việt Nam chỉ cho thu nhập 4-6 triệu/tháng trong khi cô từng được trả 30 triệu khi làm ở Nhật.'
    },
    {
        title: 'Tràn lan video "ngắn và nhảm"',
        img: 'https://i1-sohoa.vnecdn.net/2022/08/02/reels-1659433801-1659433814-1703-1659434379.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=74Ieu_6pE0MVaWf7kRGjCQ',
        description: 'Nhiều người dùng TikTok, Reels chạy đua thực hiện nội dung "câu view", trong khi các nền tảng video ngắn cũng không mạnh tay kiểm duyệt.'
    },
    {
        title: 'Chàng trai làm nghề "phù phép" những bức tường',
        img: 'https://i1-giadinh.vnecdn.net/2022/08/07/tranh-3d-24-1659805429-1659805-9666-2784-1659806168.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=QJqIRVEEEcMAl96pX8TMeg',
        description: 'TP HCMNhững bức tường nhà khô khan, cũ kỹ, qua bàn tay Đức Dự sẽ biến thành bức tranh 3D khổ lớn mà nếu không nhìn kỹ, nhiều người lầm tưởng đó là cảnh thật. '
    },
    {
        title: 'Lò huấn luyện lính Ukraine của cựu binh phương Tây',
        img: 'https://i1-vnexpress.vnecdn.net/2022/08/05/7701-1659691256-7013-1659691600.jpg?w=220&h=132&q=100&dpr=1&fit=crop&s=Dgsunsd72yOf3yAsnFrqmg',
        description: 'Các cựu binh từ Mozart Group tự nhận sứ mệnh của họ là tăng cường sức mạnh cho quân đội Ukraine, thay vì trực tiếp cầm súng trên chiến trường. '
    }
]

</script>

<style scoped>
ul {
    list-style-type: none;
}

.main-section {
    display: flex;
    padding: 20px 0;
    border-bottom: 1px solid #757575;
}

.col-left {
    width: 400px;
    border-right: 1px solid #757575;
    padding-right: 20px;
}

.col-left ul{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.col-left ul li {
    margin-bottom: 12px;
    border-bottom: 1px solid #757575;
}

.col-left ul li:last-child {
    border: none;
}

.col-right {
    width: 700px;
    padding-left: 20px;
}

</style>