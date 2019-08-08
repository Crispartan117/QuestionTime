<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light my-navbar">
        <div class="container">
            <router-link :to="{ name: 'home' }" class="navbar-brand">QuestionTime</router-link>
            <div class="collapse navbar-collapse">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item active">
                        <router-link :to="{ name: 'home' }" class="btn btn-sm btn-success">Home</router-link>
                    </li>
                    <li class="nav-item active mx-1">
                        <router-link :to="{ name: 'about' }" class="btn btn-sm btn-danger">About</router-link>
                    </li>
                    <li class="nav-item">
                        <a class="btn btn-sm btn-outline-secondary" href="/accounts/logout/">Logout</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a
                            class="nav-link dropdown-toggle"
                            href="#"
                            id="navbarDropdown"
                            role="button"
                            data-toggle="dropdown"
                            aria-haspopup="true"
                            aria-expanded="false"
                        >Dropdown</a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a class="dropdown-item" href="#">Action</a>
                            <a class="dropdown-item" href="#">Another action</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Something else here</a>
                        </div>
                    </li>
                    <li class="nav-item">
                        <a
                            class="nav-link disabled"
                            href="#"
                            tabindex="-1"
                            aria-disabled="true"
                        >Disabled</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: "NavbarComponent"
};
</script>

<style>
    .my-navbar {
        border-bottom: 1px solid #ddd;
    }
    .navbar-brand {
        font-weight: bold;
        font-size: 130%;
    }
    .navbar-brand:hover {
        color: #dc3545 !important;
    }
</style>
