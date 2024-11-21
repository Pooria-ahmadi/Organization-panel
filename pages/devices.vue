<template>
    <div class="max-width-1160px" style="width: 100%;">
        <div class="columns box mx-0 mt-0 mb-4 height-box-600px">
            <div class="column">
                <p class="has-text-black">
                    دستگاه ها
                </p>
                <p>
                    سوال یا نظری دارید؟ برای ما پیامتان را بفرستید.
                </p>
                <p class="mt-75">
                    تعداد دستگاه ها : 2
                </p>
                <div class="columns mx-0 my-5">
                    <div class="column br-15px-grey has-text-centered has-text-black mb-0 mt-2 mx-3">
                        <img src="hood.png" alt="">
                        <p>
                            B 2032 U
                        </p>
                        <p class="my-3">
                            شماره سریال : 123456789
                        </p>
                        <p>
                            وضعیت:
                            <strong class="has-text-success">
                                روشن
                                <span class="dot has-background-success"></span>
                            </strong>
                        </p>
                    </div>
                    <div class="column br-15px-grey has-text-centered has-text-black mb-0 mt-2 mx-3">
                        <img src="hood.png" alt="">
                        <p>
                            B 2032 U
                        </p>
                        <p class="my-3">
                            شماره سریال : 123456789
                        </p>
                        <p>
                            وضعیت:
                            <strong class="has-text-danger">
                                خاموش
                                <span class="dot-danger has-background-danger"></span>
                            </strong>
                        </p>
                    </div>
                    <div class="column br-15px-grey has-text-centered mt-2 mx-3 is-align-content-center">
                       <p class="has-text-info">
                        افزودن دستگاه
                       </p>
                       <img src="icons8-plus-24.png" alt="" class="mt-3">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style>
.dot {
  height: 10px;
  width: 10px;
  border-radius: 50%;
  display: inline-block;
}
.dot-danger {
  height: 10px;
  width: 10px;
  border-radius: 50%;
  display: inline-block;
}
@media only screen and (min-width: 1024px) {
    .height-box-600px{
    height: 600px;
}
}
</style>
