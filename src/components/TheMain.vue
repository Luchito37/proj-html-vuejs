<template>
    <div>
        <BuildBusiness></BuildBusiness>

        <LetDream1></LetDream1>

        <LetDream2></LetDream2>

        <LetDream3></LetDream3>

        <YouTubeVideo></YouTubeVideo>

        <UpcomingEvents></UpcomingEvents>

        <LoveSection></LoveSection>

        <SezioneProva></SezioneProva>

        <SubNews></SubNews>

        <TheFooter></TheFooter>
    </div>
</template>


<script>
import BuildBusiness from './BuildBusiness.vue';
import LetDream1 from './LetDream1.vue';
import LetDream2 from './LetDream2.vue';
import LetDream3 from './LetDream3.vue';
import YouTubeVideo from './YouTubeVideo.vue';
import UpcomingEvents from './UpcomingEvents.vue';
import LoveSection from './LoveSection.vue';
import SubNews from './SubNews.vue';
import TheFooter from './TheFooter.vue';
import SezioneProva from './SezioneProva.vue';


export default {
    name: 'App',
    components: {
    BuildBusiness,
    LetDream1,
    LetDream2,
    LetDream3,
    YouTubeVideo,
    UpcomingEvents,
    LoveSection,
    SubNews,
    TheFooter,
    SezioneProva
    

    }
}
</script>

<style scoped lang="scss">

</style>
