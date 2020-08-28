<template>
    <section class="stat">
        <div class="stat-container">
            <h2 class="stat-head">Advanced Statistics</h2>
            <p class="stat-text">
                 Track how your links are performing across the web with <br>
                 our advanced statistics dashboard 
            </p>
            <div class="stat-card-container">
                <div class="stat-card card-a">
                    <div class="stat-icon icon-a">
                        <img :src="require('@/assets/icon-brand-recognition.svg')" alt="">
                    </div>
                    <h3 class="stat-card-head">
                        Brand Recognition
                    </h3>
                    <p class="stat-card-text">
                        Boost your brand recognition with each click. Generic links don't mean a thing. Branded links helps instill confidence in your content.
                    </p>
                </div>
                <div class="stat-card card-b">
                    <div class="stat-icon icon-b">
                        <img :src="require('@/assets/icon-detailed-records.svg')" alt="">
                    </div>
                    <h3 class="stat-card-head">
                        Detailed Records
                    </h3>
                    <p class="stat-card-text">
                        Gain insights into who is clicking your links. Knowing when and where people engage with your content helps inform better decisions.
                    </p>
                </div>
                <div class="stat-card card-c">
                    <div class="stat-icon icon-c">
                        <img :src="require('@/assets/icon-fully-customizable.svg')" alt="">
                    </div>
                    <h3 class="stat-card-head">
                        Fully Customizable
                    </h3>
                    <p class="stat-card-text">
                        Improve brand awareness and content discoverability through customizable links, supercharging audience engagement.
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:"Statistics"
}
</script>

<style scoped>
    .stat{
        background-color: rgb(240,241,246);
        margin-top: 7rem;
        padding: 0 0 5rem 0;
    }

    .stat-container {
        padding: 7rem;
    }

    .stat-head {
        text-align: center;
        font-size: 2.5rem;
        color: hsl(260, 8%, 14%);
        margin-top: 7rem;
    }

    .stat-text {
        text-align: center;
        color: hsl(0, 0%, 75%)
    }

    .stat-card-container {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        margin-top: 5rem;
    }

    .stat-card {
        width: 22%;
        background: #fff;
        padding: 2rem;
        border-radius: 3%;
        position: relative;
        top: 0;
    }



    .stat-card.card-b::before {
        display: block;
        content: "";
        position: absolute;
        top: 45%;
        left: -15%;
        height: 3%;
        width: 15%;
        background: hsl(180, 66%, 49%);
        z-index: 1;
    }

    .stat-card.card-b::after {
        display: block;
        content: "";
        position: absolute;
        top: 45%;
        left: 100%;
        height: 3%;
        width: 15%;
        background: hsl(180, 66%, 49%);
        z-index: 1;
    }

    .stat-icon {
        background: hsl(255, 11%, 22%);
        position: absolute;
        top: -10%;
        height: auto;
        width: 15%;
        padding: 1.1rem;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .stat-icon img {
        position: relative;
        margin: 0 auto;
    }


    .card-a {
        position: relative;
        top: 0;
    }

    .card-b {
        position: relative;
        top: 4rem;
    }

    .card-c {
        position: relative;
        top: 8rem;
    }

    .stat-card-head {
        margin-top: 3rem;
    }

    .stat-card-text {
        font-size: 1rem;
        color: hsl(0, 0%, 75%);
    }
</style>