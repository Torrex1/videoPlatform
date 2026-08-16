<template>
    <div class="header__search">
        <div class="header__search-container">
            <input type="text">
            <img src="~/assets/search.svg" alt="searchLogo">
        </div>
    </div>
    
</template>

<style>
    .header__search {
        position: relative;
        width: 100%;
        max-width: 30%;
    }

    .header__search-container {
        position: relative;
        width: 100%;
    }

    .header__search-container > input {
        width: 100%;
        padding: 10px 12px 10px 35px;
        border: 1px solid #ccc;
        border-radius: 6px;
        outline: none;

        font-size: 18px;
    }

    .header__search-container > img {
        position: absolute;
        width: 16px;
        height: 16px;
        
        top: 50%;
        transform: translateY(-50%);
        left: 12px;
        
        pointer-events: none; 
    }
</style>