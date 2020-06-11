<template>
    <div>
        <HeaderAuth />
        <card value="text" />
    </div>
</template>

<script>
import HeaderAuth from "../components/HeaderAuth";
import Card from "../components/Card";
export default {
    data() {
        return {
            text: "ログイン"
        };
    },
    components: {
        HeaderAuth,
        Card
    }
};
</script>

<style scoped>
button {
    width: 100px;
    text-align: center;
    padding: 8px 0 10px;
    color: #fff;
    background-color: #5419da;
    border-radius: 25px;
    cursor: pointer;
}

.card {
    margin: 100px auto;
    width: 350px;
    background: #fff;
    border-radius: 5px;
    padding: 20px;
}
.card p {
    color: black;
    font-weight: bold;
    text-align: center;
}

input {
    margin-top: 15px;
    width: 80%;
    border-radius: 10px;
    padding: 10px;
    border: 1px solid black;
    color: black;
}

.form {
    text-align: center;
}
.form button {
    margin-top: 15px;
}


@media screen and (max-width: 480px) {
.card {
    margin: 100px 20px;
    width: 80%;
}
}
</style>