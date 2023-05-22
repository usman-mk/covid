<template>
    <nav class="navbar navbar-expand-md navbar-dark navbar-default">
        <!-- <div class="container"> -->
            <nuxt-link to="/" class="navbar-brand">Nuxt</nuxt-link>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item active">
                        <nuxt-link to="/" class="nav-link">หน้าหลัก <span class="sr-only">(current)</span></nuxt-link>
                    </li>
                    <li class="nav-item">
                        <nuxt-link to="/posts" class="nav-link">โพสต์</nuxt-link>
                    </li>
                </ul>
            </div>
        <!-- </div> -->
    </nav>
</template>
