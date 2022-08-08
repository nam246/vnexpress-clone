<template>
  <nav class="nav">
    <ul class="parent">
        <li><span class="material-icons">home</span></li>
        <li>Thoi su</li>
        <li>Goc nhin</li>
        <li>The gioi</li>
        <li>Video</li>
        <li>Podcasts</li>
        <li>Kinh doanh</li>
        <li>Khoa hoc</li>
        <li>Giai tri</li>
        <li>The thao</li>
        <li>Phap luat</li>
        <li>Giao duc</li>
        <li>Suc khoe</li>
        <li>Doi song</li>
        <li>Du lich</li>
        <li>So hoa</li>
        <li>Xe</li>
        <li>Y kien</li>
        <li>Tam su</li>
        <li>Hai</li>
        <li>Tat ca <span class="material-icons">menu</span></li>
    </ul>
  </nav>
  <hr>
</template>

<script>
export default {

}
</script>

<style scoped>
.nav {
    position: sticky;
}

.parent {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    list-style: none;
    padding: 0 15px;
    font-size: 14px;
    font-weight: 600;
}

.parent li {
    padding: 16px 0;
}

.parent li:first-child span{
    background-color: grey;
    border-radius: 50%;
}

.parent li:first-child span:hover {
    background-color: brown;
    color: #fff;
}

.parent li:last-child {
    display: flex;
    align-items: center;
    color: #757575;
}

.parent li:last-child:hover {
    color: brown;
}
</style>