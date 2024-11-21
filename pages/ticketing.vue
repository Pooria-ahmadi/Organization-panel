<template>
    <div style="overflow: hidden;">
        <div class="max-width-1160px mx-auto">
            <template>
  <div class="box chat-box" style="max-width: 400px; margin: auto;">

    <div class="level">
      <div class="level-left">
        <figure class="image is-48x48">
          <img src="usericon.png" alt="تصویر کوچک">
        </figure>
        <div class="ml-4">
          <p class="has-background-primary has-text-white p-2 mb-2">متن نمونه</p>
          <p class="is-size-5 has-text-weight-bold">23</p>
        </div>
      </div>
    </div>

    <!-- گزینه‌ها -->
    <div class="buttons are-small mt-3">
      <button
        v-for="(option, index) in options"
        :key="index"
        class="button is-primary has-text-white"
        @click="selectOption(option)"
      >
        {{ option }}
      </button>
    </div>

    <!-- پیام چت -->
    <div v-if="selectedOption" class="chat-message mt-4">
      <div class="has-text-centered">
        <p class="has-background-primary has-text-white p-2 mb-2">{{ selectedOption }}</p>
      </div>
      <div class="has-text-left">
        <p class="has-background-light p-2 mt-2">متن خودکار در اینجا</p>
      </div>
    </div>

    <!-- ورودی -->
    <div class="field mt-4">
      <div class="control has-icons-right">
        <input
          class="input"
          type="text"
          placeholder="متن خود را وارد کنید"
        >
        <span class="icon is-right">
          <img src="usericon.png" alt="آیکون کوچک" />
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      options: ["گزینه ۱", "گزینه ۲", "گزینه ۳", "گزینه ۴"],
      selectedOption: null,
    };
  },
  methods: {
    selectOption(option) {
      this.selectedOption = option;

      // تأخیر برای نمایش متن خودکار
      setTimeout(() => {
        this.selectedOption = "متن خودکار در سمت چپ!";
      }, 1000);
    },
  },
};
</script>

<style>
.chat-box {
  border-radius: 10px;
  padding: 1.5rem;
}

.chat-message {
  animation: fadeIn 0.5s ease-in-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

        </div>
    </div>
</template>
<script>
export default {
    head() {
        return {
            title: ' تیکتینگ',
        }
    },
}
</script>
<style>
.br-red-10 {
    border: 1px solid #fd8f8f;
    border-radius: 10px;
}
</style>