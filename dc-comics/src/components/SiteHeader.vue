<script>

export default {
    name: 'SiteHeader',
    data (){
        return {
            menu:[
                {
                    text:'Characters'
                },
                {
                    text:'Comics'
                },
                {
                    text:'Movies'
                },
                {
                    text:'Tv'
                },
                {
                    text:'Games'
                },
                {
                    text:'collectibles'
                },
                {
                    text:'videos'
                },
                {
                    text:'fans'
                },
                {
                    text:'news'
                },
                {
                    text:'shop'
                },
            ]
        }
    }

}

</script>


<template>

    <header id="site_header">
        <div class="container">
            <!-- logo -->
            <div class="col">

                <div class="logo">
                    <!-- immagine -->
                    <img src="/img/dc-logo.png" alt="brand-logo"> 
                </div>
            </div>         
            <!-- navbar -->
            <div class="col">
                <nav class="navbar">
                    <ul>    
                        <!-- list item per ogni link -->
                        <li v-for="item in menu">
                            <a href="#">{{ item.text }}</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

</template>


<style scoped>

header {
    height:100px;
    background-color: white;
}

.container {
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
    justify-content: space-between;
    height: 100%;
}

.navbar ul {
    display: flex;
    justify-content: space-between;
    list-style: none;
    gap: 0.5rem;
    align-items: center;
}

a{
    text-decoration: none;
    color:cadetblue;
    text-transform: uppercase;
}

.logo{
    display: flex;
    align-items: center;
}
img{
    width: 50px;
}


</style>