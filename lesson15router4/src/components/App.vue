<template>
    <div id="app">
        <h1>Named Routes</h1>
        <p>Current route name: {{ $route.name }}</p>
        <ul>
            <li>
                <router-link :to="{ name: 'home' }">home</router-link>
            </li>
            <li>
                <router-link :to="{ name: 'foo' }">foo</router-link>
            </li>
            <li>
                <router-link :to="{ name: 'bar', params: { id: 123 }}">bar</router-link>
            </li>
        </ul>
        <router-view></router-view>
    </div>
</template>
<script>
export default {

}
</script>
