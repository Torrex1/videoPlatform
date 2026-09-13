<script setup lang="ts">
    import { Search } from "~/shared/ui/search";
</script>

<template>
    <div class="header">
        <div class="header__logo">
            <img src="" alt="logo">
        </div>

        <!-- todo: пока так, потом в отдельный слой features где будет еще и логика поиска  -->
        <Search />

        <ul class="header__list">
            <!-- todo: отдельный слой features или entities -->
            <li class="header__list-notification">
                <img src="~/assets/notification.png" alt="icon">
            </li>

            <!-- todo: отдельный слой features -->
            <li class="header__list-profile">
                <span>RT</span>
            </li>
        </ul>
    </div>
</template>

<style>
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;

        background-color: #fff;
    }

    .header__list {
        display: flex;
        flex-direction: row;
        gap: 20px;
    }

    .header__list-notification > img {
        width: 16px;
        cursor: pointer;
    }

    .header__list-profile > span {
        border-radius: 50%;
        padding: 14px;

        background-color: #a8abbae6;
        color: #ffffff;
        cursor: pointer;
    }

</style>