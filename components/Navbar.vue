<template>
    <div class="navbar">
        <div class="navbar__title">
            Список новостей
            <div class="navbar__update">
                <img src="@/assets/navbar/update.png" alt="logo">
            </div>
        </div>
       
        <div class="navbar__search">
			<input type="search" class="navbar__search">
			<button class="navbar__btn" type="submit"><img src="@/assets/navbar/search.svg" alt="logo"></button>
		</div>
    </div>
</template>

<style lang="scss">
.navbar {
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;
    font-size: 36px;
    padding: 36px 0;
    user-select: none;
    border-bottom: solid 1px #E5E5E5;
    margin: 0 170px;

    &__title {
        display: flex;
        gap: 30px;
    }

    &__update {
        display: flex;
        width: 20px;
        height: 16px;
        padding: 12px 10px;
        border-radius: 50%;
        box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.05), 0px 1px 4px rgba(0, 0, 0, 0.05);

        img {
            width: 100%;
            height: 100%;
        }
    }

    &__search {
        display: flex;
        position: relative;
        width: 321px;
        height: 40px;
        input, button {
            border: none;
            outline: none;
            border-radius: 3px;
        }
        input {
            font-size: 18px;
            box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.05), 0px 1px 4px rgba(0, 0, 0, 0.05);
        }
        input[type="search"]::-webkit-search-cancel-button {
	        margin-right: 40px;
            cursor: pointer;
        }
        button {
            position: absolute;
            right: 15px;
            top: 0;
            bottom: 0;
            justify-content: left;
            cursor: pointer;
            background: none;
            width: 20px;
        }
    }
}
</style>