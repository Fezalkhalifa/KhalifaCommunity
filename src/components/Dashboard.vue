<template>
  <!--Container -->
  <div class="mx-auto bg-grey-400">
    <!--Screen-->
    <div class="min-h-screen flex flex-col">
      <!--Header Section Starts Here-->
      <header class="bg-nav">
        <div class="flex justify-between">
          <div class="p-2 mx-3 inline-flex items-center">
            <i class="fas fa-bars pr-2 text-white" @click="sidebarToggle()"></i>
            <h1 class="text-white p-2">Logo</h1>
          </div>
          <div class="p-2 flex flex-row items-center">
            <img @click="profileToggle()" class="inline-block h-8 w-8 rounded-full"
              src="https://therichpost.com/wp-content/uploads/2021/03/avatar2.png" alt="" />
            <a href="#" @click="profileToggle()" class="text-white p-2 no-underline hidden md:block lg:block">Jassa The
              Rich</a>
            <div id="ProfileDropDown" class="
                rounded
                hidden
                shadow-md
                bg-white
                absolute
                pin-t
                mt-12
                mr-1
                pin-r
              ">
              <ul class="list-reset ">
                <li>
                  <a href="#" class="
                      no-underline
                      px-4
                      py-2
                      block
                      text-black
                      hover:bg-grey-light
                    ">My account</a>
                </li>
                <li>
                  <a href="#" class="
                      no-underline
                      px-4
                      py-2
                      block
                      text-black
                      hover:bg-grey-light
                    ">Notifications</a>
                </li>
                <li>
                  <hr class="border-t mx-2 border-grey-ligght" />
                </li>
                <li>
                  <a href="#" class="
                      no-underline
                      px-4
                      py-2
                      block
                      text-black
                      hover:bg-grey-light
                    ">Logout</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </header>
      <!--/Header-->

      <div class="flex flex-1">
        <!--Sidebar-->
        <aside id="sidebar" class="
            bg-side-nav
            w-1/2
            md:w-1/6
            lg:w-1/6
            border-r border-side-nav
            hidden
            md:block
            lg:block
          ">
          <ul class="list-reset flex flex-col">
            <li class="
                w-full
                h-full
                py-3
                px-2
                border-b border-light-border
                bg-white
              ">
              <a href="/" class="
                  font-sans font-hairline
                  hover:font-normal
                  text-sm text-nav-item
                  no-underline
                ">
                <i class="fas fa-tachometer-alt float-left mx-2"></i>
                Dashboard
                <span><i class="fas fa-angle-right float-right"></i></span>
              </a>
            </li>
            <li class="w-full h-full py-3 px-2">
              <a href="#" class="
                  font-sans font-hairline
                  hover:font-normal
                  text-sm text-nav-item
                  no-underline
                ">
                <i class="far fa-file float-left mx-2"></i>
                Pages
                <span><i class="fa fa-angle-down float-right"></i></span>
              </a>
              <ul class="list-reset -mx-2 bg-white-medium-dark">
                <li class="
                    border-t
                    mt-2
                    border-light-border
                    w-full
                    h-full
                    px-2
                    py-3
                  ">
                  <router-link class="
                      mx-4
                      font-sans font-hairline
                      hover:font-normal
                      text-sm text-nav-item
                      no-underline
                    " to="/login">Login Page
                    <span><i class="fa fa-angle-right float-right"></i></span>
                  </router-link>
                </li>
                <li class="border-t border-light-border w-full h-full px-2 py-3">
                  <router-link class="
                      mx-4
                      font-sans font-hairline
                      hover:font-normal
                      text-sm text-nav-item
                      no-underline
                    " to="/register">Register Page
                    <span><i class="fa fa-angle-right float-right"></i></span>
                  </router-link>
                </li>
              </ul>
            </li>
          </ul>
        </aside>
        <!--/Sidebar-->
        <!--Main-->
        <main class="bg-white-300 flex-1 p-3 overflow-hidden">
          <div class="flex flex-col">
            <!-- Stats Row Starts Here -->
            <div class="flex flex-1 flex-col md:flex-row lg:flex-row mx-2">
              <div class="
                  shadow-lg
                  bg-red-vibrant
                  border-l-8
                  hover:bg-red-vibrant-dark
                  border-red-vibrant-dark
                  mb-2
                  p-2
                  md:w-1/4
                  mx-2
                ">
              </div>

              <div class="
                  shadow
                  bg-info
                  border-l-8
                  hover:bg-info-dark
                  border-info-dark
                  mb-2
                  p-2
                  md:w-1/4
                  mx-2
                ">
                <div class="p-4 flex flex-col">
                  <a href="#" class="no-underline text-white text-2xl">
                    199.4
                  </a>
                  <a href="#" class="no-underline text-white text-lg">
                    Total Funds
                  </a>
                </div>
              </div>

              <div class="
                  shadow
                  bg-warning
                  border-l-8
                  hover:bg-warning-dark
                  border-warning-dark
                  mb-2
                  p-2
                  md:w-1/4
                  mx-2
                ">
                <div class="p-4 flex flex-col">
                  <a href="#" class="no-underline text-white text-2xl"> 900 </a>
                  <a href="#" class="no-underline text-white text-lg">
                    Total Users
                  </a>
                </div>
              </div>

              <div class="
                  shadow
                  bg-success
                  border-l-8
                  hover:bg-success-dark
                  border-success-dark
                  mb-2
                  p-2
                  md:w-1/4
                  mx-2
                ">
                <div class="p-4 flex flex-col">
                  <a href="#" class="no-underline text-white text-2xl"> 500 </a>
                  <a href="#" class="no-underline text-white text-lg">
                    Total Products
                  </a>
                </div>
              </div>
            </div>

            <!-- /Stats Row Ends Here -->

            <!-- Card Sextion Starts Here -->
            <div class="flex flex-1 flex-col md:flex-row lg:flex-row mx-2">
              <div class="rounded overflow-hidden shadow bg-white mx-2 w-full">
                <div class="px-6 py-2 border-b border-light-grey">
                  <div class="font-bold text-xl text-center">User Details</div>
                </div>
                <div class="table-responsive">
                  <table class="table text-grey-darkest" ref="table">
                    <thead class="bg-grey-dark text-white text-normal">
                      <tr>
                        <th scope="col">#</th>
                        <th scope="col">Name</th>
                        <th scope="col">Email</th>
                        <th scope="col">Address</th>
                        <th scope="col">City</th>
                        <th scope="col">ZIP</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr v-for="(item,index) in allUsers" :key="item.registrationId">
                        <td>{{index+1}}</td>
                        <td>
                          <button class="
                              bg-blue-500
                              hover:bg-blue-800
                              text-white
                              font-light
                              py-1
                              px-2
                              rounded-full
                            ">
                            {{item.name}}
                          </button>
                        </td>
                        <td>{{item.email}}</td>
                        <td>{{item.address}}</td>
                        <td>
                        {{item.city}}
                        </td>
                        <td>
                        {{item.zip}}
                        </td>
                        <td rowspan="6" v-if="item==null||!item"></td>
                      </tr>
                    </tbody>
                  </table>
                </div>
              </div>
              <!-- /card -->
            </div>
            <!-- /Cards Section Ends Here -->

            <!-- Progress Bar -->
            <div class="flex flex-1 flex-col md:flex-row lg:flex-row mx-2 mt-2">
              <div class="rounded overflow-hidden shadow bg-white mx-2 w-full pt-2">
                <div class="px-6 py-2 border-b border-light-grey">
                  <div class="font-bold text-xl">Progress Among Projects</div>
                </div>
                <div class="">
                  <div class="w-full">
                    <div class="shadow w-full bg-grey-light">
                      <div class="
                          bg-blue-500
                          text-xs
                          leading-none
                          py-1
                          text-center text-white
                        " style="width: 45%">
                        45%
                      </div>
                    </div>

                    <div class="shadow w-full bg-grey-light mt-2">
                      <div class="
                          bg-teal-500
                          text-xs
                          leading-none
                          py-1
                          text-center text-white
                        " style="width: 55%">
                        55%
                      </div>
                    </div>

                    <div class="shadow w-full bg-grey-light mt-2">
                      <div class="
                          bg-orange-500
                          text-xs
                          leading-none
                          py-1
                          text-center text-white
                        " style="width: 65%">
                        65%
                      </div>
                    </div>

                    <div class="shadow w-full bg-grey-300 mt-2">
                      <div class="
                          bg-red-800
                          text-xs
                          leading-none
                          py-1
                          text-center text-white
                        " style="width: 75%">
                        75%
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--Profile Tabs-->
            <div class="
                flex flex-1 flex-col
                md:flex-row
                lg:flex-row
                mx-2
                p-1
                mt-2
                lg:mx-2
                md:mx-2
                justify-between
              ">
              <!--Top user 1-->
              <div class="
                  rounded rounded-t-lg
                  overflow-hidden
                  shadow
                  max-w-xs
                  my-3
                ">
                <img src="https://therichpost.com/wp-content/uploads/2021/04/flip-3.jpg" alt="" class="w-full" />
                <div class="flex justify-center -mt-8">
                  <img src="https://therichpost.com/wp-content/uploads/2021/03/avatar8.png" alt="" class="
                      responsvie-img
                      rounded-full
                      border-solid border-white border-2
                      -mt-3
                    " />
                </div>
                <div class="text-center px-3 pb-6 pt-2">
                  <h3 class="text-black text-sm bold font-sans">
                    Olivia Dunham
                  </h3>
                  <p class="mt-2 font-sans font-light text-grey-700">
                    Hello, i'm from another the other side!
                  </p>
                </div>
                <div class="flex justify-center pb-3 text-grey-dark">
                  <div class="text-center mr-3 border-r pr-3">
                    <h2>34</h2>
                    <span>Photos</span>
                  </div>
                  <div class="text-center">
                    <h2>42</h2>
                    <span>Friends</span>
                  </div>
                </div>
              </div>
              <!--Top user 2-->
              <div class="
                  rounded rounded-t-lg
                  overflow-hidden
                  shadow
                  max-w-xs
                  my-3
                ">
                <img src="https://therichpost.com/wp-content/uploads/2021/04/flip-3.jpg" alt="" class="w-full" />
                <div class="flex justify-center -mt-8">
                  <img src="https://therichpost.com/wp-content/uploads/2021/03/avatar8.png" alt="" class="
                      responsvie-img
                      rounded-full
                      border-solid border-white border-2
                      -mt-3
                    " />
                </div>
                <div class="text-center px-3 pb-6 pt-2">
                  <h3 class="text-black text-sm bold font-sans">
                    Olivia Dunham
                  </h3>
                  <p class="mt-2 font-sans font-light text-grey-dark">
                    Hello, i'm from another the other side!
                  </p>
                </div>
                <div class="flex justify-center pb-3 text-grey-dark">
                  <div class="text-center mr-3 border-r pr-3">
                    <h2>34</h2>
                    <span>Photos</span>
                  </div>
                  <div class="text-center">
                    <h2>42</h2>
                    <span>Friends</span>
                  </div>
                </div>
              </div>
              <!--Top user 3-->
              <div class="
                  rounded rounded-t-lg
                  overflow-hidden
                  shadow
                  max-w-xs
                  my-3
                ">
                <img src="https://therichpost.com/wp-content/uploads/2021/04/flip-3.jpg" alt="" class="w-full" />
                <div class="flex justify-center -mt-8">
                  <img src="https://therichpost.com/wp-content/uploads/2021/03/avatar8.png" alt="" class="
                      responsvie-img
                      rounded-full
                      border-solid border-white border-2
                      -mt-3
                    " />
                </div>
                <div class="text-center px-3 pb-6 pt-2">
                  <h3 class="text-black text-sm bold font-sans">
                    Olivia Dunham
                  </h3>
                  <p class="mt-2 font-sans font-light text-grey-dark">
                    Hello, i'm from another the other side!
                  </p>
                </div>
                <div class="flex justify-center pb-3 text-grey-dark">
                  <div class="text-center mr-3 border-r pr-3">
                    <h2>34</h2>
                    <span>Photos</span>
                  </div>
                  <div class="text-center">
                    <h2>42</h2>
                    <span>Friends</span>
                  </div>
                </div>
              </div>
            </div>
            <!--/Profile Tabs-->
          </div>
        </main>
        <!--/Main-->
      </div>
      <!--Footer-->
      <footer class="bg-grey-darkest text-white p-2">
        <div class="flex flex-1 mx-auto">&copy; 2021</div>
        <div class="flex flex-1 mx-auto">
          Distributed by:
          <a href="https://therichpost.com/" target=" _blank">Jassa</a>
        </div>
      </footer>
      <!--/footer-->
    </div>
  </div>
</template>
<script>
export default {
  data:function(){
    allUsers:[]
  },
  methods: {
    sidebarToggle() {
      var sidebar = document.getElementById("sidebar");

      if (sidebar.style.display === "none") {
        sidebar.style.display = "block";
      } else {
        sidebar.style.display = "none";
      }
    },
    profileToggle() {
      var profileDropdown = document.getElementById("ProfileDropDown");
      if (profileDropdown.style.display === "block") {
        profileDropdown.style.display = "none";
      } else {
        profileDropdown.style.display = "block";
      }
    },
    GetAllUsers:  function () {
      let uri = 'https://khalifacommunityapi.azurewebsites.net/Registration';
      this.axios.get(uri, this.ticket).then((response) => {
        if (response.data != null) {
          var data = response.data;
          if (data.messageType == 1) {
            this.$nextTick(() => {
            this.allUsers = data.result;
            });
            this.allUsers = data.result;
            console.log(data.result);
            this.$forceUpdate();
          }
        }
      });
    }
  },
  mounted: function () {
    this.GetAllUsers();
  }

};
</script>