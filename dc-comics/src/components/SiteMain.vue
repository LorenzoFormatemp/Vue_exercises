<script>

import comics from '../assets/data/comics';
import AppHero from './AppHero.vue';
import ComicItem from './ComicItem.vue';

export default {
    name: 'SiteMain',
    components : {
        AppHero,
        ComicItem
    },
    data () {
        return {
            comics: comics
        }
    }
}


</script>


<template>

    <main id="site_main">
        
        <div class="content">

            <!-- Jumbotron -->
            <AppHero/>

            <div class="container">
                <!--  comicItem-->
                <ComicItem v-for="comic in comics"
                    :img="comic.thumb"
                    :title="comic.series"
                />
            
            </div>

        </div>

        <!-- bannerBannerItem -->
    </main>



</template>
