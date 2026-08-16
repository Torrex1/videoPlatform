<script setup lang="ts">
    import { Search } from "~/shared/ui";
</script>

<template>
    <div class="header">
        <div class="header__logo">
            <img src="" alt="logo">
        </div>

        <Search />

        <ul class="header__list">
            <li class="header__list-notification">
                <img src="~/assets/notification.png" alt="icon">
            </li>
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
        width: 20px;
        border-radius: 50%;
        border: 1px solid #ccc;
        padding: 14px;
        cursor: pointer;
    }

</style>