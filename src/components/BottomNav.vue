<template>

    <div class="container-fluid">
        <div class="row">
            <div class="col-4">
                <img class="logo" src="../assets/GCNLogo.svg" />
            </div>
            <div class="col-8">
                <div class="scoailIcons text-end">
                    <a href="https://facebook.com/globalcyclingnetwork"><i class="bi bi-facebook ico"></i></a>
                    <a href="https://twitter.com/gcntweet"><i class="bi bi-twitter ico"></i></a>
                    <a href="https://instagram.com/globalcyclingnetwork/?hl=en"><i class="bi bi-instagram ico"></i></a>
                </div>
            </div>
        </div>
        <div class="row archive">
            <div class="col"></div>
            <div class="col-2">
                <ul>
                    <li class="itms"><a href="">See full archive</a></li>
                    <li class="itms"><a href="">Auguest 2022</a></li>
                    <li class="itms"><a href="">July 2022</a></li>
                    <li class="itms"><a href="">June 2022</a></li>
                    <li class="itms"><a href="">May 2022</a></li>
                    <li class="itms"><a href="">April 2022</a></li>
                    <li class="itms"><a href="">March 2022</a></li>
                </ul>
            </div>
            <div class="col-2">
                <ul>
                    <li class="itms"><a href="">February 2022</a></li>
                    <li class="itms"><a href="">January 2022</a></li>
                    <li class="itms"><a href="">December 2021</a></li>
                    <li class="itms"><a href="">November 2021</a></li>
                    <li class="itms"><a href="">October 2021</a></li>
                    <li class="itms"><a href="">September 2021</a></li>
                    <li class="itms"><a href="">Auguest 2021</a></li>
                </ul>
            </div>
            <div class="col-2">
                <ul>
                    <li class="itms"><a href="">July 2021</a></li>
                    <li class="itms"><a href="">June 2021</a></li>
                    <li class="itms"><a href="">May 2021</a></li>
                    <li class="itms"><a href="">April 2021</a></li>
                    <li class="itms"><a href="">March 2021</a></li>
                    <li class="itms"><a href="">February 2021</a></li>
                    <li class="itms"><a href="">Januray 2021</a></li>
                </ul>
            </div>
            <div class="col-2">
                <ul>
                    <li class="itms"><a href="">December 2020</a></li>
                    <li class="itms"><a href="">November 2020</a></li>
                    <li class="itms"><a href="">October 2021</a></li>
                    <li class="itms"><a href="">September 2020</a></li>
                    <li class="itms"><a href="">Auguest 2020</a></li>
                    <li class="itms"><a href="">July 2022</a></li>
                    <li class="itms"><a href="">June 2020</a></li>
                </ul>
            </div>
            <div class="col-2">
                <ul>
                    <li class="itms"><a href="">May 2022</a></li>
                    <li class="itms"><a href="">April 2020</a></li>
                </ul>

            </div>
            <div class="col"></div>
        </div>

        <a class="btn btn-sm btn-outline-danger" href="https://www.globalcyclingnetwork.com/archive/full/"
            role="button">See full archive</a>
        <div class="row">
            <div class="col-12">


                <span class="separator"><a href="http://www.playsportsnetwork.com/">© 2022 Play Sports Network</a></span>
                <span class="separator"> | <a href="http://www.playsportsnetwork.com/">Home</a></span>
                <span class="separator"> | <a href="http://www.playsportsnetwork.com/">Editorial Policy</a></span>
                <span class="separator"> | <a href="http://www.playsportsnetwork.com/">Privacy Policy</a></span>
                <span class="separator"> | <a href="http://www.playsportsnetwork.com/">Cookie Policy</a></span>
                <span class="separator"> | <a href="http://www.playsportsnetwork.com/">California Do Not Sell My
                        Personal Info</a></span>

            </div>

        </div>

        <a class="btn btn-sm btn-outline-success"
            href="https://www.globalcyclingnetwork.com/video/punchy-finish-makes-for-late-attacking-tour-of-scandinavia-2022-stage-6-highlights"
            role="button">Manage Preferences</a>

    </div>

</template>

<script>
export default {
    name:"BottomNav"
}
</script>

<style scoped>

.container-fluid {
    padding-bottom: 20px;
    background-color: black;
}

.logo {
    width: 150px;
    height: 150px;
    margin-left: 80px;
}

.scoailIcons {
    margin-top: 45px;
    margin-right: 80px;
}

.ico {
    color: white;
    padding: 10px;
    font-size: 20px;
}

.itms {
    color: white;
    font-size: 0.9rem;
}

a {
    text-decoration: none;
    color: white;
}


ul {
    list-style-type: none;
}

.separator {
    color: white;
    font-size: 0.7rem;
}


@media only screen and (max-width: 992px){
.archive{
    display: none;
}
.logo{
    margin-left: 0px;
    width: 100px;
    height: 100px;
}

.scoailIcons{
    margin-top: 35px;
    margin-right:0px;
}

}

</style>