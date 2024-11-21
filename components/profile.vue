<template>
  <div class="is-hidden-mobile is-hidden-tablet-only">
    <div class="menu-container w-100-z-index-2 box columns is-vcentered py-2 mt-5">
      <div class="column has-text-right is-flex is-align-items-self-start">
        <img src="Profile 1.png" alt="">
        <p class="pr-2 has-text-black has-text-weight-bold">
          پوریا احمدی
        </p>
      </div>
      <div class="column py-0">
        <div class="columns is-mobile is-vcentered is-justify-content-end">
          <div class="column py-0 is-flex is-justify-content-end">
            <div class="is-flex pl-4 hover-background" style="width: 205px;">
              <NuxtLink to="/login" class="is-flex">
                <img class="pl-4" src="icons8-log-out-24.png" alt="">
                <p>خروج از حساب کاربری</p>
              </NuxtLink>
            </div>
          </div>
          <div class="column is-1">
            <img src="Notification 2.png" alt="" class="pt-2">
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>
.fixed-box {
  width: 100%;
  height: 700px;
  background-color: #f5f5f5;
  border: 1px solid #ddd;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 135px;
}

.hover-background:hover {
  background-color: #ff3860;

  padding: 5px;
  border-radius: 4px;
}

.hover-background:hover p {
  color: white;
}

.menu-hover {
  position: relative;
}

.menu-icon {
  transition: opacity 0.3s ease;
  position: relative;
  z-index: 1;
}

.menu-hover:hover .menu-icon {
  opacity: 0;
}

.hover-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-150%, -50%);
  background-color: #5468B1;
  color: white;
  padding: 5px 10px;
  border-radius: 4px;
  opacity: 0;
  transition: opacity 0.3s ease, transform 0.5s ease;
  white-space: nowrap;
  z-index: 0;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  min-width: 100px;
}

.logout-hover :hover {
  color: white;
  background-color: rgb(212, 27, 14);
}

.menu-hover:hover .hover-text {
  opacity: 1;
  transform: translate(-50%, -50%);
}
</style>