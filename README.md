<!DOCTYPE html>
<html>

<head>
    <title>Forget Form</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
    <link rel="stylesheet" type="text/css" href="style.css" />
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" />
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
    <link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" />
</head>

<body>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-6 col-md-6 d-none d-md-block image-container"></div>

            <div class="col-lg-6 col-md-6 form-container">
                <div class="col-lg-8 col-md-12 col-sm-9 col-xs-12 form-box">
                    <div class="text-center logo mb-3">
                        <h1><b>THE CURREN TIMES</b></h1>
                    </div>
                    <div class="reset-form d-block">
                        <form class="reset-password-form">
                            <h4 class="mb-3">Reset your password</h4>
                            <p class="mb-3 text-white">Please enter your email address</p>
                            <div class="form-input">
                                <span><i class="fa fa-envelope"></i></span>
                                <input type="email" placeholder="Email Address" required />
                            </div>
                            <div class="mb-3">
                                <button class="btn" type="submit">Send Reset Code</button>
                            </div>
                        </form>
                    </div>
                    <div class="reset-confirmation d-none">
                        <div class="mb-4">
                            <h4 class="mb-3">Link was send</h4>
                            <h6 class="text-black">Please check your inbox</h6>
                        </div>
                        <div>
                            <a href="login.html">
                                <button type="submit" class="btn">Login Now</button>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script type="text/javascript">
        function PasswordReset() {
            $("form.reset-password-form").on("submit", function(e) {
                e.preventDefault();
                $(".reset-form").removeClass("d-block").addClass("d-none");

                $(".reset-confirmation").addClass("d-block");
            });
        }

        window.addEventListener("load", function() {
            PasswordReset();
        });
    </script>
</body>

</html>
