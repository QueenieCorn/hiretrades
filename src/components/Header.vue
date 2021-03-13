<template>
    <div>
        <b-navbar toggleable="lg" align-v="left" class="px-md-3 p-2">
            <b-navbar-brand href="#" class="p-0">
                <router-link to="/">
                    <img alt="comp icon" class="pr-2" src="../assets/comp-icon.png">
                    <img alt="comp logo text" src="../assets/comp-logo.png">
                </router-link>
                </b-navbar-brand>

            <b-navbar-toggle target="nav-collapse" class="queenie"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav>
                <b-nav-item to="/some/route/" exact exact-active-class="active">Trades</b-nav-item>
                <b-nav-item to="/some/route/" exact exact-active-class="active">Cost Guides</b-nav-item>
                <b-nav-item to="/some/route/" exact exact-active-class="active">Blog</b-nav-item>
            </b-navbar-nav>

            <!-- Right aligned nav items -->
            <b-navbar-nav class="ml-auto">
                 <b-nav-item to="/some/route/" exact exact-active-class="active">Get Qoutes</b-nav-item>
                 <b-nav-item class="btn-register"><b-button variant="outline-primary" class="py-2 px-4">Register Business</b-button></b-nav-item>
                 <b-nav-item to="/some/route/" exact exact-active-class="active">Login</b-nav-item>
            </b-navbar-nav>
            </b-collapse>
        </b-navbar>
</div>
</template>

<style scoped lang="scss">
$font-stack:    Helvetica, sans-serif;

body{
    font-family: "IBM Plex Sans",Helvetica,Arial,serif;
    color: #666!important;
    font-size: 16px;
    font-weight: 400;
}
nav {
    border-bottom: 1px solid #dfe3e7;
    padding:0 20px;
    .nav-item{
        font-weight: 800;
        a{
            color: #666;
            text-decoration: none;
            border-bottom: 1px solid transparent !important;
            &:hover{
                color: #7367F0;
                border-bottom: 1px solid #7367F0 !important;
            }
        }
    }
    .navbar-toggler-icon{
        background-image:url('../assets/menu-toggle.png') !important;
    }

    .btn-register {
        a {
            padding: 10px 0;
            &:hover{
                border-bottom: 1px solid transparent !important;
            }
        }
    }
    .navbar-toggler.queenie  {
        // background: red !important;
        border: none;
        font-size: 15px;
    }

    @media only screen and (max-width: 767px) {
        padding: 10px;
    }

}

.navbar-nav .nav-item a{
         @media only screen and (max-width: 767px) {
        padding: 10px;
        }
    }

     

</style>
