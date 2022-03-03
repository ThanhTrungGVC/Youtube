<template>
    <div class="sidebar">
        <div class="menu">
            <router-link to="/"><img src="@/assets/home.png" alt=""><p>Home</p></router-link>
            <router-link to="/"><img src="@/assets/explore.png" alt=""><p>Explore</p></router-link>
            <router-link to="/"><img src="@/assets/subscriprion.png" alt=""><p>Subscriprion</p></router-link>
            <router-link to="/"><img src="@/assets/library.png" alt=""><p>Library</p></router-link>
            <router-link to="/"><img src="@/assets/history.png" alt=""><p>History</p></router-link>
            <router-link to="/"><img src="@/assets/playlist.png" alt=""><p>PlayList</p></router-link>
            <router-link to="/"><img src="@/assets/messages.png" alt=""><p>Messages</p></router-link>
            <router-link to="/"><img src="@/assets/show-more.png" alt=""><p>More</p></router-link>
            <hr>
        </div>

        <div class="subcribed">
            <h3>SUBCRIBED</h3>
            <a href=""><img src="@/assets/Jack.png" alt=""><p>Jack Nicholson</p></a>
            <a href=""><img src="@/assets/simon.png" alt=""><p>Simon Baker</p></a>
            <a href=""><img src="@/assets/tom.png" alt=""><p>Tom Hardy</p></a>
            <a href=""><img src="@/assets/megan.png" alt=""><p>Megan Ryan</p></a>
            <a href=""><img src="@/assets/cameron.png" alt=""><p>Cameron Diaz</p></a>
        </div>
    </div>
</template>

<script>
export default {
  name: "Sidebar"
};
</script>

<style>

.sidebar{
    padding-left: 2%;
    padding-top: 25px;
    position: fixed;
    top: 55px;
    background: #fff;
    width: 15%;
    height: 100%;
}

.menu a{
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    width: fit-content;
    flex-wrap: wrap;
}

.menu a:first-child{
    color: #ed3833;
}

.menu a img{
    width: 20px;
    margin-right: 20px;
}

.sidebar hr{
    border: 0;
    height: 1px;
    background: #ccc;
    width: 85%;
}

.subcribed h3{
    font-size: 13px;
    margin: 20px 0;
}

.subcribed a{
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    width: fit-content;
    flex-wrap: wrap;
}

.subcribed a img{
    width: 25px;
    border-radius: 50%;
    margin-right: 20px;
}
</style>
