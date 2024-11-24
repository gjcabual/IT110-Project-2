<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import RegisterForm from '@/components/auth/RegisterForm.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto">
          <v-card class="mx-auto" prepend-icon=" mdi-account-plus" subtitle="Sign Up">
            <template v-slot:title>
              <span class="font-weight-black">ToolBucks</span>
            </template>

            <v-card-text class="pt-4">
              <RegisterForm></RegisterForm>

              <v-divider class="my-5"></v-divider>

              <h5 class="text-center">
                Already have account?
                <RouterLink class="text-decoration-none" to="/">Click here to Login</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
