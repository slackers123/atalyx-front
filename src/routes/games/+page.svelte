<script>
    import { Swiper, SwiperSlide} from "swiper/svelte";
    import { Navigation } from 'swiper';
    import GameSwipe from "$lib/GameSwipe.svelte";
    import "swiper/css";
    import "swiper/css/navigation"
    import GameThumb from "$lib/GameThumb.svelte";

</script>

<div class="swiper">
    <div class="prev_el">
        <img src="arrow.svg" alt="next element">
    </div>
    <div class="next_el">
        <img src="arrow.svg" alt="next element">
    </div>
    <Swiper
    modules={[Navigation]}
    slidesPerView={1}
    navigation={{
        nextEl: ".next_el",
        prevEl: ".prev_el"
    }}
    >
        <SwiperSlide><GameSwipe title="A Monk's Tale" link="/games/a-monks-tale" src="sc1.png"/></SwiperSlide>
        <SwiperSlide><GameSwipe title="High Up" link="/games/high-up" src="sc1.png"/></SwiperSlide>
        <SwiperSlide><GameSwipe title="Fatigue" link="/games/fatigue" src="sc1.png"/></SwiperSlide>
    </Swiper>
</div>
<div class="games">
    <div class="games-content">
        <h2>Upcoming</h2>
        <div class="games-list" style="width: 25%;">
            <GameThumb title="A Monk's Tale 2" />
        </div>
        <h2>Released</h2>
        <div class="games-list">
            <GameThumb title="A Monk's Tale"/>
            <GameThumb title="A Monk's Tale"/>
            <GameThumb title="High UP" src="highup.png" link="/games/high-up"/>
            <GameThumb title="Fatigue" src="fatigue.png"link="/games/fatigue"/>
        </div>
    </div>
</div>

<style>

    .games-list {
        display: flex;
    }

    h2 {
        font-size: 2.5rem;
    }

    .next_el {
        position: absolute;
        top: 50%;
        right: 1rem;
        z-index: 5;
        transform: translate(0, -50%);
    }

    .prev_el {
        position: absolute;
        top: 50%;
        left: 1rem;
        transform: rotate(180deg) translate(0, 50%);
        z-index: 5;
    }

    .swiper {
        height: 50vh;
        width: 100vw;
    }

    .games {
        background-color: rgba(234, 255, 255, 0.39);
        width: 100vw;
        height: fit-content;
    }
    
    .games-content {
        margin-left: 8vw;
        margin-right: 8vw;
        padding-left: 3vw;
        padding-top: 5vw;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        background-color: white;
        height: 100vh;
    }
</style>