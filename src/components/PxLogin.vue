<template>
  <div class="min-h-full flex items-center justify-center py-12 px-4 sm:px-6 lg:px-8">
    <div class="max-w-md w-full space-y-8">
      <div>
        <img class="mx-auto h-12 w-auto" src="https://rahabogados.com.mx/wp-content/uploads/2016/01/man-2.png" alt="Workflow">
        <h2 class="mt-6 text-center text-3xl font-extrabold text-amber-400">Iniciar sesión</h2>
        <p class="mt-2 text-center text-sm text-gray-600">
          Un
          <a href="#" class="font-medium text-amber-400 hover:text-amber-500"> texto de prueba </a>
        </p>
      </div>
      <form v-on:submit.prevent="onSubmit" class="mt-8 space-y-6" action="#" method="POST">
        <input type="hidden" name="remember" value="true">
        <div class="rounded-md shadow-sm -space-y-px">
          <div>
            <label for="email-address" class="sr-only">Dirección de correo electrónico</label>
            <input v-model="email" id="email-address" name="email" type="email" autocomplete="email" required class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm" placeholder="Dirección de correo electrónico">
          </div>
          <div>
            <label for="password" class="sr-only">Contraseña</label>
            <input v-model="password" id="password" name="password" type="password" autocomplete="current-password" required class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-b-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm" placeholder="Contraseña">
          </div>
        </div>

        <div class="flex items-center justify-between">
          <div class="flex items-center">
            <input id="remember-me" name="remember-me" type="checkbox" class="h-4 w-4 text-amber-400 focus:ring-amber-500 border-gray-300 rounded">
            <label for="remember-me" class="ml-2 block text-sm text-gray-900"> Recordar </label>
          </div>

          <div class="text-sm">
            <a href="#" class="font-medium text-amber-400 hover:text-amber-500"> ¿Has olvidado tu contraseña? </a>
          </div>
        </div>

        <div>
          <button @click="iniciarSesion" type="submit" class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-amber-400 hover:bg-amber-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-amber-500">
            <span class="absolute left-0 inset-y-0 flex items-center pl-3">
              <!-- Heroicon name: solid/lock-closed -->
              <svg class="h-5 w-5 text-white-500 group-hover:text-white-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                <path fill-rule="evenodd" d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z" clip-rule="evenodd" />
              </svg>
            </span>
            Iniciar Sesión
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PxLogin',
  props: {

  },
  data() {
    return {
      email: "",
      password: ""
    };
  },
  methods: {
    iniciarSesion() {
      
    }
  }
}
</script>
