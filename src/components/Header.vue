<template>
  <div class="header">
    <div class="container">
        <div class="top-header">
            <div class="left">
                <span class="logo">
                    <img src="https://s1.vnecdn.net/vnexpress/restruct/i/v631/v2_2019/pc/graphics/logo.svg" alt="">
                </span>
                <span class="seperate">|</span>
                <span class="time">Saturday, 6/8/2022</span>
            </div>
            <div class="right">
                <div class="newest">
                    <span class="material-icons">schedule</span><span>Newest</span>
                </div>
                <div class="evne">
                    <p>International</p>
                </div>
                <span class="seperate">|</span>
                <div class="search-bar">
                    <input type="search" placeholder="Search">
                    <span class="material-icons">search</span>
                </div>
                <div class="signin">
                    <span class="material-icons">person</span>
                    <span>Sign in</span>
                </div>
            </div>
        </div>
    </div>
  </div>
  <hr>
</template>

<script>
export default {

}
</script>

<style scoped>
.header {
    padding: 8.5px 0;
}

.top-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.left {
    display: flex;
    align-items: center;
    justify-content: center;
}

.logo {
    margin-right: 20px;
}

.time {
    margin-left: 20px;
    font-size: 14px;
}

.right {
    display: flex;
}



.newest, .evne {
    display: flex;
    align-items: center;
    border: 1px solid grey;
    padding: 0 10px;
    line-height: 30px;
    margin: 0 15px;
    font-size: 14px;
}

.search-bar {
    position: relative;
    margin-left: 15px;
}

.search-bar input {
    height: 32px;
    width: 160px;
    line-height: 32px;
    border-radius: 16px;
    border: 1px solid grey;
    outline: none;
    padding: 0 30px 0 14px;
}

.search-bar .material-icons {
    position: absolute;
    right: 8px;
    top: 4px;
}

.signin {
    display: flex;
    align-items: center;
    margin-left: 20px;
}
</style>