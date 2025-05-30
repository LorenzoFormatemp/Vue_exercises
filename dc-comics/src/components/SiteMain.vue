<script>

import comics from '../assets/data/comics';
import AppHero from './AppHero.vue';
import ComicItem from './ComicItem.vue';
import BannerItem from './BannerItem.vue';

export default {
    name: 'SiteMain',
    components : {
        AppHero,
        ComicItem,
        BannerItem
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

            <!--  comicItem-->
            <div class="container">
                <ComicItem v-for="comic in comics"
                    :img="comic.thumb"
                    :title="comic.series"
                />
            </div>

        </div>

        <!-- BannerItem -->
        <BannerItem/>
    </main>



</template>
