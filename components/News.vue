<template>
    <div class="news">
        <div class="news__all">
            Все
        </div>
        <div class="news__lenta">
            Lenta.ru
        </div>
        <div class="news__mos">
            Mos.ru
        </div> 
    </div>
</template>

<style lang="scss">
.news {
    display: flex;
    gap: 10px;
    font-size: 14px;
    margin: 25px 170px;
    user-select: none;

    &__all, &__lenta, &__mos {
        cursor: pointer;
        color: #0029FF;
    }

     &__all:hover, &__lenta:hover, &__mos:hover {
        color: #000000;
    }
}
</style>