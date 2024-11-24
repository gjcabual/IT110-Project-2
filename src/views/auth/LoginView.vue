<script setup>
import LoginForm from '@/components/auth/LoginForm.vue'
import AppLayout from '@/components/layout/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto">
          <v-card class="mx-auto" subtitle="Sign In">
            <v-card-title class="text-center">
              <v-img src="/public/images/cgear.png" width="150" class="mx-auto"></v-img>
              <h3 class="font-weight-black">TOOLBUCKS</h3>
            </v-card-title>
            <v-card-text class="bg-surface-light pt-4">
              <v-divider class="my-5"></v-divider>
              <LoginForm></LoginForm>

              <v-divider class="my-5"></v-divider>

              <h5 class="text-center">
                Don't have account?
                <RouterLink class="text-decoration-none" to="/register"
                  >Click here to Register</RouterLink
                >
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
