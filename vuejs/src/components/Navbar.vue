<template>
    <!-- ------------ Phần navbar header ------------ -->
    <nav class="div-flex">
        <!-- ------------ Phần header trái: Menu icon + Logo icon ------------ -->
        <div class="nav-left div-flex">
            <img src="@/assets/menu.png" alt="" class="menu-icon">
            <img src="@/assets/logo.png" alt="" class="logo-icon">
        </div>
        
        <!-- ------------ Phần header giữa: Thanh tìm kiếm ------------ -->
        <div class="nav-center div-flex">
            <div class="search-box div-flex">
                <input type="text" placeholder="Nhập nội dung tìm kiếm">
                <img src="@/assets/search.png" alt="">
            </div>

            <img src="@/assets/voice-search.png" alt="" class="search-voice">
        </div>

        <!-- ------------ Phần header phải: Thông báo, Tài khoản ------------ -->
        <div class="nav-right div-flex">
            <img src="@/assets/upload.png" alt="">
            <img src="@/assets/more.png" alt="">
            <img src="@/assets/notification.png" alt="">
            <img src="@/assets/Jack.png" alt="" class="account-icon">
        </div>
    </nav>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style>

nav{
    padding: 10px 2%;
    justify-content: space-between;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    background: #fff;
    position: sticky;
    z-index: 10;
    top: 0;
    height: 55px;
    width: 100%;
}

.nav-left .menu-icon{
    width: 22px;
    margin-right: 25px;
}

.nav-left .logo-icon{
    width: 130px;
}

.nav-center .search-box {
    border: 1px solid #ccc;
    border-radius: 25px;
    padding: 8px 12px;
    margin-right: 15px;
}

.nav-center .search-box img {
    width: 15px;
}

.nav-center .search-box input{
    border: 0;
    width: 400px;
    background: transparent;
    outline: 0;
}

.nav-center .search-voice{
    width: 16px;
}

.nav-right img{
    width: 25px;
    margin-right: 25px;
}

.nav-right .account-icon{
    width: 35px;
    margin-right: 0;
    border-radius: 50%;
}
</style>
