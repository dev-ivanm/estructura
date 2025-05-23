<template>
  <div class="flex items-center justify-center min-h-screen">
    <div class="grid grid-cols-2 gap-4">
      <div class="row-span-2 flex items-center justify-center">
        <a
          href="#"
          class="block w-[600px] max-w-sm px-10 py-8 bg-white border border-gray-200 rounded-lg shadow-sm hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
        >
          <img
            class="w-38 h-38 mx-auto mb-4 rounded-full shadow-lg"
            src="https://dummyimage.com/400x400/000/fff"
            alt="Bonnie image"
          />

          <h5
            class="mb-4 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
          >
            Mi perfil
          </h5>

         <template>
    <div class="flex items-center justify-center min-h-screen p-12"> 
      <div class="grid grid-cols-2 gap-4 w-full max-w-4xl">
        <div class="flex items-center p-4 bg-white border border-gray-200 rounded-lg shadow-sm hover:bg-gray-100 dark:bg-gray-800">
          <div class="p-3 mr-4 rounded-full">
            <img
              class="w-38 h-38 mx-auto mb-4 rounded-full shadow-lg"
              src="https://dummyimage.com/400x400/000/fff"
              alt="image"
            />
          </div>
          <div>
            <h4 class="mb-2 font-bold text-gray-600 dark:text-gray-400">Mi perfil</h4>
            <ul class="text-sm font-medium text-gray-600 max-w-md space-y-2 list-none list-inside dark:text-gray-400 mb-4">
              <li><strong>Nombre:</strong> Ivan Mendoza</li>
              <li><strong>Cargo:</strong> Developer</li>
              <li><strong>Registrado desde:</strong> 12/03/2025</li>
            </ul>
  
            <div class="flex justify-left space-x-2">
              <button
                type="button"
                class="text-white bg-blue-700 hover:bg-blue-800 font-medium rounded-full text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
              >
                Volver al inicio
              </button>
  
              <button
                type="button"
                class="py-2.5 px-5 text-sm font-medium text-gray-900 bg-white rounded-full border border-gray-200 hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-100 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
              >
                Gestionar contraseña
              </button>
  
              <button
                type="button"
                class="py-2.5 px-5 text-sm font-medium text-gray-900 bg-white rounded-full border border-gray-200 hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-100 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
              >
                Salir
              </button>
            </div>
          </div>
        </div>
  
        <div class="flex items-center p-4 bg-white border border-gray-200 rounded-lg shadow-sm hover:bg-gray-100 dark:bg-gray-800">
          <div class="p-3 mr-4 text-orange-500 bg-orange-100 rounded-full dark:text-orange-100 dark:bg-orange-500">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
              <path
                d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3zM6 8a2 2 0 11-4 0 2 2 0 014 0zM16 18v-3a5.972 5.972 0 00-.75-2.906A3.005 3.005 0 0119 15v3h-3zM4.75 12.094A5.973 5.973 0 004 15v3H1v-3a3 3 0 013.75-2.906z"
              ></path>
            </svg>
          </div>
          <div>
            <p class="mb-2 text-sm font-medium text-gray-600 dark:text-gray-400">Total clients</p>
            <p class="text-lg font-semibold text-gray-700 dark:text-gray-200">6389</p>
          </div>
        </div>
      </div>
    </div> 
  </template>  


        </a>
      </div>

      <div class="flex items-center justify-center">
        <a
          href="#"
          class="block w-[600px] max-w-sm p-6 bg-white border border-gray-200 rounded-lg shadow-sm hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
        >
          <h5
            class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
          >
            Informacion de la empresa 
          </h5>
          <ul
            class="max-w-md space-y-2 text-gray-500 list-none list-inside dark:text-gray-400 mb-4"
          >
            <li><strong>Nombre de la empresa:</strong> Wanted Inc</li>
            <li><strong>Categoria:</strong> N/A</li>
            <li><strong>Numero de polizas:</strong> 12</li>
            <li><strong>Precio por usuario:</strong> $50.000</li>
            <li><strong>Total usuarios:</strong> 3</li>
            <li><strong>Costo mensual aprox.:</strong> $150.000</li>
          </ul>

          <div class="flex justify-left space-x-2">
            <button
              type="button"
              class="text-white bg-blue-700 hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-full text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
            >
              Volver al inicio
            </button>

            <button
              type="button"
              class="py-2.5 px-5 text-sm font-medium text-gray-900 focus:outline-none bg-white rounded-full border border-gray-200 hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-100 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
            >
              Cerrar sesión
            </button></div>
        </a>
      </div>
      <div class="col-start-2 row-start-2 flex items-center justify-center">
        <a
          href="#"
          class="block w-[600px] max-w-sm p-6 bg-white border border-gray-200 rounded-lg shadow-sm hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
        >
          <h5
            class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
          >
            Gestonar contraseñas
          </h5>
          <div>
            <label
              for="small-input"
              class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
              >Nueva contraseña</label
            >
            <input
              type="text"
              id="small-input"
              class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
            />
          </div>
          <div>
            <label
              for="small-input"
              class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
              >Confirmar contraseña</label
            >
            <input
              type="text"
              id="small-input"
              class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
            />
          </div>
          <div class="flex justify-left mt-5">
            <button
              type="button"
              class="text-white bg-blue-700 hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-full text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
            >
              Actualizar
            </button>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.grid {
  grid-template-columns: auto auto;
}
</style>
