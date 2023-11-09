<template lang="">
    <div class="container">
        <img src="@/assets/logo-white.png" class="logo-white"/>
        <img class="download-example" src="@/assets/download-example.png"/>
        <Button class="download-btn" @click="downloadFile">
            <span>下载健康守护星APP</span>
        </Button>
        <img class="download-qr" src="@/assets/download-qr.png"/>
        <div class="download-txt">扫码下载</div>
    </div>
</template>

<script setup>
    const downloadFile = () => {
        const link = 'https://0000.0000.apk'; //다운로드 링크
        window.location.href = link;
    }
</script>

<style lang="scss" scoped>
    .container {
        height:1024px;
        width:768px;
        background-size: cover;
        background-image: url("~@/assets/download-background.png");
    }

    .logo-white {
        height:61px;
        width:96px; 
        object-fit: cover;
        position:absolute;
        padding: 100px 0 0 320px;
    }

    .download-example {
        padding: 200px 0 0 20px;
        width:675px; 
        height:551px;
        object-fit: cover;
    }

    .download-btn {
        width: 460px;
        height: 80px;
        position:absolute;
        right: 140px;
        top: 820px;
        color: white;
        background: linear-gradient(180deg, #6DD8E8, #3BAFCC);
        border-radius: 44.5px;
        border: none;
        font-size: 24px;
        font-weight: 500;
    }

    .download-qr {
        width:112px; 
        height:112px;
        padding: 100px 0 0 35px;
    }

    .download-txt {
        font-size: 16px;
        font-weight: 500;
        color: white;
        padding: 0 0 0 35px;
    }
</style>
