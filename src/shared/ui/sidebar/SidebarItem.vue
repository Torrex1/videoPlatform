<script lang="ts" setup >
defineProps<{
    itemText: string;
    linkTo?: string;
}>();
</script>

<template>
    <li class="sidebar__list-item sidebar__item">
        <img class="sidebar__item-icon" src="../../../assets/search.svg" alt="itemIcon">
        <a class="sidebar__item-link" :href="linkTo">{{ itemText }}</a>
    </li>
</template>

<style scoped>
    .sidebar__list-item {
        display: flex;
        gap: 10px;

        padding: 20px;
        border: 1px solid #e4e4e4ab;
        border-radius: 10px;
        cursor: pointer;
    }
    .sidebar__item-icon {
        width: 16px;
    }
    .sidebar__item-link {
        font-size: 18px;
    }

    .sidebar__list-item:hover {
        box-shadow: 2px 5px 8px 1px #d8d8d865;
    }
    .sidebar__list-item:active {
        box-shadow: unset;
    }
</style>