<template>

  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <img class="logoImg" src="../assets/GCNLogo.svg" alt="gcn_logo" />
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <img id="logo" class="mobileLogo" src="../assets/GCNLogo.svg" alt="gcn_logo" />
      <input id="searchBar" class="searchBar" type="search" placeholder="Search" aria-label="Search">
      <i id="openbtn" class="bi bi-search ms-auto" @click="showSearchBar()"></i>
      <i id="closebtn" class="bi bi-x-lg ms-auto closebtn" @click="closeSearchBar()"></i>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="https://www.globalcyclingnetwork.com/category/gcn-show">GCN
              Show</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/how-to">How to</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/maintenance-mondays">Maintenance</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/ask-gcn">Ask GCN</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/train-with-gcn">Training</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/features">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/top-10s">Top 10s</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/gcn-racing">GCN Racing</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.globalcyclingnetwork.com/category/gcn-tech">GCN Tech</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Presenters
            </a>
            <ul class="dropdown-menu bg-dark">
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/conor-dunne">Connor
                  Dunne</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/daniel-lloyd">Daniel
                  LLoyd</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/james-lw">James
                  Lowsley-Williams</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/jon-cannings">Jon
                  Cannings</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/manon-lloyd">Mannon
                  LLoyd</a></li>
              <li><a class="dropdown-item"
                  href="https://www.globalcyclingnetwork.com/presenters/oliver-bridgewood">Oliver Bridgewood</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/simon-richardson">Simon
                  Richardson</a></li>
              <li><a class="dropdown-item" href="https://www.globalcyclingnetwork.com/presenters/tom-last">Tom Last</a>
              </li>
            </ul>
          </li>
          <li>
            <button class="btn icobtn" type="submit">
              <i class="bi bi-search ico"></i>
            </button>
          </li>
        </ul>
        <!-- <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form> -->
      </div>
    </div>
  </nav>
</template>

<script>
export default {
    name:"Header",
    data(){

      return{
        isShown: false
      }

    },mounted(){
      
    },methods:{
      showSearchBar(){
        if(this.isShown == false){
          console.log(this.isShown);
          document.getElementById("searchBar").style.display = "block"
          document.getElementById("logo").style.display = "none"
          document.getElementById("closebtn").style.display = "block"
          document.getElementById("openbtn").style.display = "none"
          this.isShown = true
        }
      },
      closeSearchBar(){
        if(this.isShown == true){
          console.log(this.isShown);
          document.getElementById("searchBar").style.display = "none"
          document.getElementById("logo").style.display = "block"
          document.getElementById("openbtn").style.display = "block"
          document.getElementById("closebtn").style.display = "none"
          this.isShown = false
        }
      }
    }
}
</script>

<style scoped>

.container {
  height: 80px;
}

.navbar {
  background-color: #C30106;
}

.nav-link {
  color: white;
}

.nav-item :hover {
  background-color: black;
  color: white;
}

.bi {
  display: none
}

.navbar-nav .nav-link.active {
  background-color: black;
  color: white;
}

.navbar-nav {
  margin-left: 200px;
}

.dropdown-item {
  color: white;
}

.logoImg {
  height: 120px;
  width: 120px;
}

.icobtn {
  background-color: #C30106;
}

.ico {
  font-size: 20px;
  font-weight: bolder;
}

.mobileLogo {
  display: none;
}

.searchBar {
  display: none;
}

.closebtn{
  display:none;
}

@media only screen and (max-width: 992px){
.mobileLogo{
  display: block;
  width: 50px;
  height: 50px;
  margin-left: 90px;
}
.searchBar{
  margin-left:20px;
  border:0;
  height: 30px;
  width: 230px;
  display: none;
}
.container{
    height: auto;
}

.navbar-nav{
    margin-left: 20px;
}

.icobtn{
    display: none;
}

.logoImg{
 display: none;
}

.bi{
  display: block;
  font-size: 25px;
}

.closebtn{
  display:none
}

}

</style>