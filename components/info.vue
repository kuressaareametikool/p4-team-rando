<template>
    <div class="info">
        <div>
            <h1>Saaremaa Muuseum</h1>
            <svg width="326" height="12" viewBox="0 0 326 12" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                <rect width="326" height="12" fill="url(#pattern0)"/>
                <defs>
                <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                <use xlink:href="#image0" transform="translate(-1.10625) scale(0.00334635 0.0909091)"/>
                </pattern>
                <image id="image0" width="960" height="11" xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA8AAAAALCAYAAACwEeRxAAAEIklEQVR4Ae3dUYRcVxzH8VBKKaHkqfSphNCnkqdQQiilhFBK6NNSSgkhT6GUUkopZSkhlBBKCaH0qSxlKEufog9x/3c27vnfc+7drVDCrd+du+NmOtmdyZ2dZOobxm527p1zzieH2V/+55w5dYo/CCCAAAIIILCUQIzjt6rSrlSe3YjBtmOw35Jnf8ZgzdyH24MUslFyux3L7Ova7WoVxu8u1egJXRzjX6drz863jzp744Sa4WURQAABBBBAAAEEEEAAAQQ2QWASEu1qDHYnuu3qaxXy61WZX1KQnX10AXercvtSoVfhN7odPCMc75Zut5LbJwfl3rl1epRl/tFMvx6ncvz5OvtAWwgggAACCCCAAAIIIIAAAi9YoGmaV1LIPyyL/KcU7J8U7GHt+WdNk732vF1T5VihMwX7JrrtzAvEya2KIb+fyvxmXYzfV/h+3vaOu0+hW2N7qh9uB8fdx/MIIIAAAggggAACCCCAAAIbKqAKrpYAV2G8pZA7qdpaOQ2GbjuV26cxZB/r2r9j9s4qhqqQvR/HF1RN7oK2TdvsLafulldvK7Du7+dnV9H24WvEYB/026xC/uPhc3xFAAEEEEAAAQQQQAABBBDYcAFVYruge1f7d7t9vNrLO31MAmk2SqEXhHuhVKFRwVTXaV+vwrPCcdM0rw7hWahKHKxMhf2idhXKhyydVpV7MhZ7Urt9O7T/Q8bOvQgggAACCCCAAAIIIIAAAisQaIri9RTsmkKrwqOWFy8a9nRdu89XB1+F/Hq3F/hBv3I68/0fKWQ/qGqs+4Z0X20vVCVul2lnI4X4rt02kKv9une4larX7VjCeEvjSMEsFvlXdV28PaSf3IsAAggggMBGCMy8Yc8/vXLmf7y55xmnfOLE/GEOMAeYA2ubA8u8yapKeljJVZVzmXuPulb7cyt/dPG4UJzcniS33yu377WMeegS6skp1PklHVilwKvXnjnM6rh/BwX0L1LYe++o8S3yHL8T8DsBc4A5wBxgDmzSHFjkvY1rEEAAAQQQ2FiBLiROA+EqQt9RGIuG4hjssZZfK5AroK9qb+/B3t6ZrsI7OZ3aH12MbpNqtduOKt9H9Z/nEEAAAQQQQAABBBBAAAEENlTgP5VRt92hy5KXpVg0FOsE6OT26+Ge4iGfzat9waryRreiPVV6BdXeZcfN9QgggAACCCCAAAIIIIAAAmsUiJ59N7s0S/tz19iFuU31Q3H7OcAhG2mp9Gxf9Xct326XOXeHdGkpdXfolvb5Th/ay5vcfm73OZd2T59H3N//O7cj/BABBBBAAAEEEEAAAQQQQOD/I6BqqIJi8vFld3/zZR6ZDqPSycyVZzfa/b2l3UsKxyEbTaq5vb1mbkX3c32m8LbGqKrxood7vcwO9A0BBBBAAIGTEPgXZSg96InBFdQAAAAASUVORK5CYII="/>
                </defs>
            </svg>
        </div>
        <div class="info-contacts">
            <div>
                <p>
                    Linnus avatud T-P 10.00-18.00<br>
                    E-post: muuseum@saaremaamuuseum.ee<br>
                    Telefon: +372 455 4463
                </p>
            </div>
            <div class="contact-english">
                <p>
                    Opening hours Tu-Su 10.00-18.00<br>
                    Email: muuseum@saaremaamuuseum.ee<br>
                    Phone: +372 455 4463
                </p>
            </div>
        </div>
    </div>
</template>
<style scoped>
    .info {
        display: flex;
        flex-direction: column;
        background-color: #2a221b;
        padding: 40px 30px 0;
        width: 1080px;
        height: 470px;
    }


    .info div h1 {
        font-family: 'Playfair Display', serif;
        color: white;
        font-weight: 200;
        font-size: 48px;
        padding-bottom: 30px;
    }

    .info-contacts {
        display: flex;
        justify-content: space-between;
        padding-top: 30px;
    }

    .info-contacts p {
        font-family: 'Oswald', sans-serif;
        color: white;
        font-size: 24px;
    }

    .contact-english {
        display: flex;
        align-items: flex-end;
        text-align: right;
    }
</style>