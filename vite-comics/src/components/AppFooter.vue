<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="top">
            <div class="container">
                <div class="row">
                    <div class="col-2">
                        <h3>Dc comics</h3>
                        <ul>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>Dc</h3>
                        <ul>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>Sites</h3>
                        <ul>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                            <li><a href="">Lorem</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom">
            <div class="call-to-action">
                <a href="">Sign-up now</a>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.top {
    background-image: url('../asets/img/footer-bg.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

    .container {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: right center;
        background-repeat: no-repeat;
    }

    h3 {
        text-transform: uppercase;
        margin: 1rem 0;
    }

    ul {
        list-style: none;
        margin: 1rem 0;

        li {
            a {
                text-decoration: none;
                color: $dc-light-dark;
            }
        }
    }
}
</style>