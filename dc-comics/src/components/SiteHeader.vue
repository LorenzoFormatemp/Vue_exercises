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
</style>