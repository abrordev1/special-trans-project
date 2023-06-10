<template>
    <div class="header-menu lg:ml-14 2xl:ml-[90px] hidden lg:block">
        <ul class="menu flex text-dark">
            <li class="font-normal 2xl:mr-14 lg:mr-6 hover:text-green lg:text-sm 2xl:text-lg cursor-pointer duration-300"
                v-for="item in menuItems" :key="item">
                <router-link :to="{ name: item.link }">
                    {{ item.name }}
                </router-link>
            </li>
        </ul>
    </div>
</template>

<script>
import menuList from '../menuList.js'

export default {
    data() {
        return {
            menuItems: menuList
        }
    }
}

</script>