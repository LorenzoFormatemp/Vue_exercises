<script>

import comics from '../assets/data/comics';
import AppHero from './AppHero.vue';


export default {
    name: 'SiteMain',
    components : {
        AppHero
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

            <AppHero/>
            <!-- container => i fumetti: ComicItem-->

        </div>

        <!-- bannerBannerItem -->
    </main>



</template>
