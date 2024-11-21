<template>
    <div class="max-width-1160px" style="width: 100%;">
        <div class="columns has-background-white mb-4 mx-0 mt-0 is-rounded-columns">
            <div class="column has-text-centered background-section">
                <div class="box login-box has-text-centered has-text-white">
                    <p class="is-size-4 has-text-weight-bold">
                        ورود
                    </p>
                    <p class="mt-2">
                        نام کاربری و رمزعبور خود را وارد کنید
                    </p>
                    <p class="mt-5"> نام کاربری </p>
                    <input class="input mt-3 br-input-white" type="text" placeholder="">
                    <p class="mt-5">رمز عبور</p>
                    <input class="input mt-3 br-input-white" type="text" placeholder="">
                    <NuxtLink to="/singup">
                        <p class="is-size-7 has-text-white my-4">
                            هنوز ثبت نام نکرده اید؟ ثبت نام کنید
                        </p>
                    </NuxtLink>
                    <NuxtLink to="/">
                        <button class="button is-rounded has-text-white px-6 pb-3 bg-transparent"> ورود </button>
                    </NuxtLink>
                </div>
            </div>
            <div class="column has-text-centered py-6">
                <p class="has-text-info is-size-5 has-text-weight-bold">
                    پشتیبانی 24 ساعته با هوش مصنوعی
                </p>
                <p class="has-text-info is-size-5 has-text-weight-bold">
                    به همراه تیکتینگ هوشمند
                </p>
                <img src="robot.png" alt="">
            </div>
        </div>
    </div>
</template>