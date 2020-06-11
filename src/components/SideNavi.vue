<template>
    <div>
        <div class="left-padding">
            <img class="logo" src="../assets/logo.png"/>
            <div class="flex icon-field" @click="$router.push('/home')">
                <img class="icon" src="../assets/home.png"/>
                <p>ホーム</p>
                </div>
            <div class="flex icon-field" @click="$router.push('/profile')">
                <img class="icon" src="../assets/profile.png"/>
                <p>プロフィール</p>
            </div>
            <div class="flex icon-field" @click="$store.dispatch('logout')">
                <img class="icon" src="../assets/logout.png"/>
                <p>ログアウト</p>
            </div>
        </div>
        <hr />
        <ShareMessage />
    </div>
</template>

<script>
import ShareMessage from "../components/ShareMessage"; export default {
    components: {
        ShareMessage
    }
};
</script>

<style scoped> 
.flex {
    display: flex;
}
.icon {
    width: 25px;
    height: 25px;
}
.detail {
    margin-left: 50px; }
.message {
    padding: 20px;
    border-bottom: solid 1px white;
    border-left: solid 1px white;
}
.name {
    font-size: 18px;
    font-weight: bold;
    margin-right: 10px;
}
.text {
    margin-top: 10px;
}
.number {
    margin-left: 10px;
    margin-right: 10px;
}
@media screen and (max-width: 480px) {
.icon {
    width: 30px;
    height: 30px;
}
.text {
    font-size: 10px; }
.message {
    border-left: none;
}
}
</style>