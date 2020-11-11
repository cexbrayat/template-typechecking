<template>
  <div class="hello" v-if="user">
    <h1>{{ user.name }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue';
import { UserModel } from '@/user.model';

export default defineComponent({
  name: 'HelloWorld',
  props: {
    user: Object as PropType<UserModel>,
  },
});
</script>
