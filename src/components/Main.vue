<template>
    <div>
        <main class="main-container">
            <div class="main-content">
                <h1 class="head-text">More than just shorter links</h1>
                <p class="lead-text">
                    Build your brand's recognition and get detailed<br>
                    insights on how your links are performing
                </p>

                <div class="action-btn">
                    <a href="#">
                        <button>Get Started</button>
                    </a>
                </div>
            </div>
            <div class="main-bg">
                <img
                    :src="require('@/assets/illustration-working.svg')"
                    alt="illustration-image"
                    class="illustration-image"
                />
            </div>
        </main>


        <Statistics />

        <section class="boost">
            <div class="boost-container">
                <h2>Boost your links today</h2>
                <div class="action-btn">
                    <a href="#">
                        <button>Get Started</button>
                    </a>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
import Statistics from './Statistics.vue';

export default {
    name: "Main",
    components: {
        Statistics
    }
}
</script>

<style scoped>
    .main-container {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 2rem 0 2rem 10rem;
    }

    .main-content {
        position: relative;
        bottom: 3rem;
    }
    
    .head-text {
        font-size: 5rem;
        font-weight: bold;
        line-height: 1;
        letter-spacing: 0;
        color: hsl(257, 27%, 26%);
        margin-bottom: 0;
    }

    .lead-text {
        width: 100%;
        font-size: 1.2rem;
        color: hsl(257, 7%, 63%);
    }

    button {
        padding: 1rem 3rem;
        border-radius: 1.5rem;
        border: none;
        cursor: pointer;
        background: hsl(180, 66%, 49%);
        font-size: 1rem;
        font-weight: bold;
        color: #fff;
    }

    button:hover {
        background: hsl(180, 65%, 67%);;
    }

    .main-bg {
        position: relative;
        right: 3rem;
    }

    .boost {
        width: 100%;
        background: hsl(260, 8%, 14%);
        background-image: url("~@/assets/bg-boost-desktop.svg");
        background-size: cover;
        background-repeat: no-repeat;
        padding: 2rem;
    }

    .boost-container {
        text-align: center;
        padding: 1rem;
    }

    .boost-container h2 {
        color: #fff;
        font-size: 2rem;
        padding: 1rem;
    }
</style>