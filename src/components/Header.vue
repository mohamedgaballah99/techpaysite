<template>
<div class="header">
    <nav class="navbar navbar-expand-lg navbar-light bg-light" style="position:fixed; top:0px; right:0px; left:0px;z-index: 9999999999999999;">
        <div class="container">
            <a class="navbar-brand" href="/"><img src="@/assets/image/TechPay.svg" width="150" height="auto" alt="logo" /></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item active">
                        <router-link to="/"><a class="nav-link">Home</a></router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/products"><a class="nav-link">Products</a></router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/sales"><a class="nav-link">Sales</a></router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/about"><a class="nav-link">About</a></router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/contact"><a class="nav-link">Contact</a></router-link>
                    </li>
                </ul>
                <div class="cart">
                    <router-link to="/fav"> <span><svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" class="bi bi-heart-fill" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z" />
                            </svg>
                            <sup class="cartnumber">3</sup>
                            </span></router-link>
                    <router-link to="/cart"><span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-bag-check-fill" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M10.5 3.5a2.5 2.5 0 0 0-5 0V4h5v-.5zm1 0V4H15v10a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V4h3.5v-.5a3.5 3.5 0 1 1 7 0zm-.646 5.354a.5.5 0 0 0-.708-.708L7.5 10.793 6.354 9.646a.5.5 0 1 0-.708.708l1.5 1.5a.5.5 0 0 0 .708 0l3-3z" /></svg><sup class="favnumber">4</sup></span></router-link>
                    <!-- Button trigger modal -->
                    <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
                        Login
                    </button>

                    <!-- Modal -->
                    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
                        <div class="modal-dialog">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLabel">Login</h5>
                                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                                </div>
                                <div class="modal-body">
                                    <form style="text-align:left">
                                        <div class="mb-3">
                                            <label  class="form-label">Email address :</label>
                                            <input type="email" id="email" class="form-control" aria-describedby="emailHelp" placeholder="Your Email">
                                            <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
                                        </div>
                                        <div class="mb-3">
                                            <label for="exampleInputPassword1" class="form-label">Password :</label>
                                            <input type="password"  id="password" class="form-control" placeholder="Your Password">
                                        </div>
                                        <div class="mb-3 form-check">
                                            <input type="checkbox" class="form-check-input" id="exampleCheck1">
                                            <label class="form-check-label" for="exampleCheck1">Check me out</label>
                                        </div>
                                        <button type="submit" class="btn btn-primary" id="login">Login</button>
                                    </form>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!--  -->
                    <!--  -->
                    <button type="button" class="btn btn-success" data-bs-toggle="modal" data-bs-target="#exampleModalm">
                        Sign Up
                    </button>

                    <!-- Modal -->
                    <div class="modal fade" id="exampleModalm" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
                        <div class="modal-dialog">
                            <div class="modal-content">
                                <div class="modal-header">
                                    <h5 class="modal-title" id="exampleModalLabel">Sign Up</h5>
                                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                                </div>
                                <div class="modal-body">
                                    <form style="text-align:left">
                                        <div class="mb-3">
                                            <label for="exampleInputPassword1" class="form-label">FullName :</label>
                                            <input type="text" class="form-control" placeholder="Your Name">
                                        </div>
                                        <div class="mb-3">
                                            <label for="exampleInputEmail1" class="form-label">Email address :</label>
                                            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp " placeholder="Your Email">
                                            <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
                                        </div>
                                        <div class="mb-3">
                                            <label for="exampleInputPassword1" class="form-label">Password :</label>
                                            <input type="password" class="form-control" placeholder="Your Password">
                                        </div>
                                        <div class="mb-3">
                                            <label for="exampleInputPassword1" class="form-label"> Confirm Password :</label>
                                            <input type="password" class="form-control" placeholder="Confirm Your Password">
                                        </div>
                                        <button class="btn btn-success">Sign Up</button>
                                    </form>
                                </div>
                                <div class="modal-footer">
                                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>

                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>

        </div>
    </nav>


</div>
</template>

<script>

export default {
    name: "Header",
};
</script>

<style lang="scss" scoped>
@import "../scss/style.scss";

/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
    .modal-content {
        width: 80% !important;
        margin: 100px auto !important;
    }
}

@media only screen and (max-width: 990px) {
    .header {
        .container {

            .collapse {
                ul {
                    // margin: 20px 0px !important;
                    margin: auto !important;
                    text-align: left !important;
                    li {
                        margin: 0px 0px 10px 17px!important;
                        text-align: left !important;
                        
                    }
                }
            }

            .cart {
                text-align: left;
                margin-left: 0px;
            }
        }
    }
}

.header {
    .navbar-light .navbar-toggler {
        color: $primary-color;
        border-color: $primary-color;
    }

    .container {
        .collapse {
            ul {
                li {
                    margin: 0px 20px;

                    a {
                        text-decoration: none !important;
                        font-size: 20px;
                        font-style: italic;
                        color: $primary-color;
                        transition: 0.5s all;

                        &:hover {
                            background-color: white;
                            border-radius: 20px;
                        }
                    }
                }
            }
        }

        .cart {
            span:last-of-type {
                margin-left: 25px;
            }

            span {
                cursor: pointer;

                sup {
                    font-weight: bold;
                    color: white;
                    background: $primary-color;
                    padding: 0px 5px 2px 3px;
                    border-radius: 10px;
                    font-size: 14px;
                    font-style: italic;
                }

                svg {
                    color: $primary-color;
                }
            }

            .btn-primary {
                margin: 0px 15px;
            }
        }

        .navbar-light .navbar-toggler {
            color: $primary-color;
            border-color: $primary-color;
        }
    }
}
</style>
