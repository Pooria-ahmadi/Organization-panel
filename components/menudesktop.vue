<template>

    <div class="max-width-1160px mb-4 is-hidden-mobile is-hidden-tablet-only">
        <div class="box width-240px ml-3">
            <NuxtLink to="/">
                <div class="is-flex dashboard-link is-justify-content-space-between" @mouseover="isHovered = true"
                    @mouseleave="isHovered = false">
                    <div class="is-flex">
                        <img src="Home 4.png" alt="">
                        <p>داشبورد</p>
                    </div>
                    <div>
                        <img src="icons8-back-24.png" alt="" :class="{ 'is-hidden': !isHovered }">
                    </div>
                </div>
            </NuxtLink>

            <NuxtLink to="/user">
                <div class="is-flex mt-4">
                    <img src="Profile Circle.png" alt="">
                    <p class="pr-4">
                        پروفایل
                    </p>
                </div>
            </NuxtLink>
            <NuxtLink to="/devices">
                <div class="is-flex mt-4">
                    <img src="Vector.png" alt="">
                    <p class="pr-4">
                        دستگاه ها
                    </p>
                </div>
            </NuxtLink>
            <NuxtLink to="/contactus">
                <div class="is-flex mt-4">
                    <img src="Home 4.png" alt="">
                    <p class="pr-4">
                        ارتباط با ما
                    </p>
                </div>
            </NuxtLink>
            <NuxtLink to="/Managealarms">
                <div class="is-flex mt-4">
                    <img src="Home 4.png" alt="">
                    <p class="pr-4">
                        پیغام ها و هشدار ها
                    </p>
                </div>
            </NuxtLink>
            <NuxtLink to="/ticketing">
                <div class="is-flex mt-4">
                    <img src="Home 4.png" alt="">
                    <p class="pr-4">
                        تیکتینگ با هوش مصنوعی
                    </p>
                </div>
            </NuxtLink>
        </div>
    </div>

</template>
<script>
export default {
  data() {
    return {
      isHovered: false,
    };
  },
};
</script>
<style>
.is-hidden {
  display: none;
}
.width-240px {
    height: 100%;
    width: 240px;
}

.dashboard-link {
    display: flex;
    align-items: center;
    padding: 8px;
    border-radius: 8px;
    transition: background-color 0.3s ease, color 0.3s ease;
}

.dashboard-link img {
    max-width: 32px;
    max-height: 32px;
    object-fit: contain;
}

.dashboard-link p {
    margin: 0;
    padding-right: 8px;
}

.dashboard-link:hover {
    background-color: #40e0d0;
    color: #007AFF;
}
</style>