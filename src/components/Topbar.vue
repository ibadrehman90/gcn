<template>
    <div class="container-fluid">
        <div class="row elms">
            <div class="col-md-8 col-sm-2">
            </div>
            <div class="col-md-4 col-sm-10">
                <div class="social">
                    <a class="sociaLinks" href="https://facebook.com/globalcyclingnetwork"><i
                            class="bi bi-facebook ico"></i></a>
                    <a class="sociaLinks" href="https://twitter.com/gcntweet"><i class="bi bi-twitter ico"></i></a>
                    <a class="sociaLinks" href="https://instagram.com/globalcyclingnetwork/?hl=en"><i
                            class="bi bi-instagram ico"></i></a>
                </div>
                <div class="btnGroup">
                    <a class="btn btn-light btn-sm" href="https://www.gcnevents.co/" role="button">Events</a>
                    <a class="btn btn-light btn-sm" href="https://www.gcnclub.com/" role="button">Club</a>
                    <a class="btn btn-light btn-sm" href="https://shop.globalcyclingnetwork.com/" role="button">Shop</a>
                    <a class="btn btn-light btn-sm"
                        href="https://www.youtube.com/subscription_center?add_user=globalcyclingnetwork"
                        role="button">YouTube</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

    name:"Topbar"

}
</script>

<style scoped>

.container-fluid{
    height: 50px;
    background-color: black;
    color:white;
}

.elms{
    padding-top: 10px;
}

.itm{
    padding: 5px;
}


.btn{
    margin-left: 5px;
}
.ico{

    padding: 7px;
}

.social{
    display:inline-block
}

.sociaLinks{
    text-decoration: none;
    color:white;
}

.btnGroup{
    display: inline-block;
    margin-left: 20px;
}

@media only screen and (max-width: 992px){

.btnGroup{
   
    margin-left: 2px;
}

}

</style>