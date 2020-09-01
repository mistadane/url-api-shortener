<template>
    <section class="shortener">
        <div class="shorten-container">
            <div class="shorten-cover">
                <form class="shorten-form">
                    <input type="text" name="shorten" placeholder="Shorten a link here...">
                    <button class="shorten-btn">Shorten it!</button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:"Shortener"
}
</script>

<style scoped>
    .shorten-container {
        position: relative;
        top: -4rem;
    }

    .shorten-cover {
        background: hsl(260, 8%, 14%);
        background-image: url("~@/assets/bg-shorten-desktop.svg");
        background-size: cover;
        background-repeat: no-repeat;
        width: 70%;
        padding: 2.5rem;
        margin: 0 auto;
        border-radius: .75rem;
    }

    .shorten-form {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
    }

    .shorten-form input {
        width: 70%;
        padding: 1.4rem;
        border-radius: .5rem;
        border: none;
        outline: none;
    }

    .shorten-form input::placeholder {
        font-size: 1.3rem;
        color: hsl(0, 0%, 75%);
    }

    .shorten-form button {
        padding: 1.2rem;
        width: 18%;
        border: none;
        border-radius: .5rem;
        background: hsl(180, 66%, 49%);
        color: #fff;
        font-size: 1.1rem;
        font-weight: 700;
        cursor: pointer;
    }

    .shorten-form button:hover {
        background: hsl(180, 65%, 67%);
    }
</style>