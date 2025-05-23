<template>
  <main class="p-12">
    <div class="grid grid-cols-1 lg:grid-cols-2 lg:grid-rows-2 gap-5">
      
        <div
          class="border border-gray-300 border-t-8 border-t-purple-400 rounded-2xl h-auto p-4 hover:shadow-2xl"
        >
          <div class="flex flex-col md:flex-row items-center">
            
            <div class="p-3 mb-4 md:mb-0 md:mr-4">
              <img
                class="w-32 h-32 rounded-full"
                src="https://flowbite.com/docs/images/people/profile-picture-3.jpg"
                alt="image"
              />
            </div>

            <div class="flex flex-col flex-1">
              <h4 class="text-2xl font-medium text-gray-600 mb-3">Mi perfil</h4>
              <ul
                class="text-sm font-medium text-gray-600 max-w-md space-y-2 list-none list-inside dark:text-gray-400 mb-4"
              >
                <li><strong>Nombre:</strong> Clara Mendoza</li>
                <li><strong>Cargo:</strong> Developer</li>
                <li><strong>Registrado desde:</strong> 12/03/2025</li>
              </ul>
              <div
                class="flex flex-col md:flex-row justify-start space-y-2 md:space-y-0 md:space-x-2"
              >
                <button
                  type="button"
                  class="text-white bg-purple-700 hover:bg-purple-800 focus:outline-none focus:ring-4 focus:ring-purple-300 font-medium rounded-full text-xs px-3 py-2.5 text-center dark:bg-purple-600 dark:hover:bg-purple-700 dark:focus:ring-purple-800"
                >
                  Volver al inicio
                </button>
                <button
                  type="button"
                  @click="openModal"
                  class="py-2.5 px-3 text-xs font-medium text-gray-900 focus:outline-none bg-white rounded-full border border-gray-200 hover:bg-orange-300 hover:text-white focus:z-10 focus:ring-4 focus:ring-gray-100 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
                >
                  Gestionar contraseña
                </button>
                <button
                  type="button"
                  class="py-2.5 px-3 text-xs font-medium text-gray-900 focus:outline-none bg-white rounded-full border border-gray-200 hover:bg-red-600 hover:text-white focus:z-10 focus:ring-4 focus:ring-gray-100 dark:focus:ring-gray-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700"
                >
                  Salir
                </button>
              </div>
            </div>
          </div>
        </div>
      <div>
      <div class="lg:col-start-1 lg:row-start-2">
        <div
          class="border border-gray-300 border-t-8 border-t-purple-400 rounded-2xl h-auto p-4 hover:shadow-2xl"
        >
          <h4 class="text-2xl font-medium text-gray-600 mb-3">
            Informacion de la empresa
          </h4>
          <ul
            class="text-sm font-medium text-gray-600 max-w-md space-y-2 list-none list-inside dark:text-gray-400 mb-4"
          >
            <li><strong>Nombre de la empresa:</strong> Wanted Inc</li>
            <li><strong>Categoria:</strong> N/A</li>
            <li><strong>Numero de polizas:</strong> 12</li>
            <li><strong>Precio por usuario:</strong> $50.000</li>
            <li><strong>Total usuarios:</strong> 3</li>
            <li><strong>Costo mensual aprox.:</strong> $150.000</li>
          </ul>
          <div class="flex justify-start">
            <button
              type="button"
              class="text-white bg-purple-700 hover:bg-purple-800 focus:outline-none focus:ring-4 focus:ring-purple-300 font-medium rounded-full text-sm px-5 py-2.5 text-center dark:bg-purple-600 dark:hover:bg-purple-700 dark:focus:ring-purple-800"
            >
              Agregar usuario
            </button>
          </div>
        </div>
      </div>

      <Modalpss :isOpen="isModalOpen" @close="closeModal" />

      </div>
      <div class="lg:row-span-2 lg:col-start-2 lg:row-start-1">
        <div
          class="border border-gray-300 border-t-8 border-t-purple-400 rounded-2xl hover:shadow-2xl h-full p-4"
        >
          <h2 class="text-2xl font-medium text-gray-600 mb-5">Usuarios</h2>
          <div class="overflow-x-auto">
            <table
              class="min-w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400"
            >
              <thead
                class="text-xs text-gray-50 uppercase bg-purple-400 dark:bg-gray-700 dark:text-gray-400"
              >
                <tr>
                  <th scope="col" class="px-6 py-3">Nombre</th>
                  <th scope="col" class="px-6 py-3">Usuario</th>
                  <th scope="col" class="px-6 py-3">Status</th>
                  <th scope="col" class="px-6 py-3">Accion</th>
                </tr>
              </thead>
              <tbody>
                <tr
                  class="bg-white border-b dark:bg-gray-800 dark:border-gray-700 border-gray-200 hover:bg-gray-50 dark:hover:bg-gray-600"
                >
                  <th
                    scope="row"
                    class="flex items-center px-6 py-3 text-gray-900 whitespace-nowrap dark:text-white"
                  >
                    <div>
                      <div class="text-base font-semibold">Sofia Camejo</div>
                    </div>
                  </th>
                  <td class="px-6 py-3">scamejo</td>
                  <td class="px-6 py-3">
                    <div class="flex items-center">
                      <div
                        class="h-2.5 w-2.5 rounded-full bg-green-500 me-2"
                      ></div>
                      Activo
                    </div>
                  </td>
                  <td class="px-6 py-3">
                    <a
                      href="#"
                      class="flex font-medium text-gray-600 hover:underline"
                    >
                      <svg
                        class="w-5 h-5 text-gray-800 dark:text-white"
                        aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg"
                        width="24"
                        height="24"
                        fill="none"
                        viewBox="0 0 24 24"
                      >
                        <path
                          stroke="currentColor"
                          stroke-linecap="square"
                          stroke-linejoin="round"
                          stroke-width="1"
                          d="M7 19H5a1 1 0 0 1-1-1v-1a3 3 0 0 1 3-3h1m4-6a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm7.441 1.559a1.907 1.907 0 0 1 0 2.698l-6.069 6.069L10 19l.674-3.372 6.07-6.07a1.907 1.907 0 0 1 2.697 0Z"
                        />
                      </svg>
                      Editar
                    </a>
                  </td>
                </tr>
                <tr
                  class="bg-white border-b dark:bg-gray-800 dark:border-gray-700 border-gray-200 hover:bg-gray-50 dark:hover:bg-gray-600"
                >
                  <th
                    scope="row"
                    class="flex items-center px-6 py-3 font-medium text-gray-900 whitespace-nowrap dark:text-white"
                  >
                    <div>
                      <div class="text-base font-semibold">Antonio Rojas</div>
                    </div>
                  </th>
                  <td class="px-6 py-3">arojas</td>
                  <td class="px-6 py-3">
                    <div class="flex items-center">
                      <div
                        class="h-2.5 w-2.5 rounded-full bg-green-500 me-2"
                      ></div>
                      Activo
                    </div>
                  </td>
                  <td class="px-6 py-3">
                    <a
                      href="#"
                      class="flex font-medium text-gray-600 hover:underline"
                    >
                      <svg
                        class="w-5 h-5 text-gray-800 dark:text-white"
                        aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg"
                        width="24"
                        height="24"
                        fill="none"
                        viewBox="0 0 24 24"
                      >
                        <path
                          stroke="currentColor"
                          stroke-linecap="square"
                          stroke-linejoin="round"
                          stroke-width="1"
                          d="M7 19H5a1 1 0 0 1-1-1v-1a3 3 0 0 1 3-3h1m4-6a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm7.441 1.559a1.907 1.907 0 0 1 0 2.698l-6.069 6.069L10 19l.674-3.372 6.07-6.07a1.907 1.907 0 0 1 2.697 0Z"
                        />
                      </svg>
                      Editar
                    </a>
                  </td>
                </tr>
                <tr
                  class="bg-white border-b dark:bg-gray-800 dark:border-gray-700 border-gray-200 hover:bg-gray-50 dark:hover:bg-gray-600"
                >
                  <th
                    scope="row"
                    class="flex items-center px-6 py-3 font-medium text-gray-900 whitespace-nowrap dark:text-white"
                  >
                    <div>
                      <div class="text-base font-semibold">Cristina Valera</div>
                    </div>
                  </th>
                  <td class="px-6 py-3">cvalera</td>
                  <td class="px-6 py-3">
                    <div class="flex items-center">
                      <div
                        class="h-2.5 w-2.5 rounded-full bg-green-500 me-2"
                      ></div>
                      Activo
                    </div>
                  </td>
                  <td class="px-6 py-3">
                    <a
                      href="#"
                      class="flex font-medium text-gray-600 hover:underline"
                    >
                      <svg
                        class="w-5 h-5 text-gray-800 dark:text-white"
                        aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg"
                        width="24"
                        height="24"
                        fill="none"
                        viewBox="0 0 24 24"
                      >
                        <path
                          stroke="currentColor"
                          stroke-linecap="square"
                          stroke-linejoin="round"
                          stroke-width="1"
                          d="M7 19H5a1 1 0 0 1-1-1v-1a3 3 0 0 1 3-3h1m4-6a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm7.441 1.559a1.907 1.907 0 0 1 0 2.698l-6.069 6.069L10 19l.674-3.372 6.07-6.07a1.907 1.907 0 0 1 2.697 0Z"
                        />
                      </svg>
                      Editar
                    </a>
                  </td>
                </tr>
                <tr
                  class="bg-white dark:bg-gray-800 hover:bg-gray-50 dark:hover:bg-gray-600"
                >
                  <th
                    scope="row"
                    class="flex items-center px-6 py-3 font-medium text-gray-900 whitespace-nowrap dark:text-white"
                  >
                    <div>
                      <div class="text-base font-semibold">Pedro Gomez</div>
                    </div>
                  </th>
                  <td class="px-6 py-3">pgomez</td>
                  <td class="px-6 py-3">
                    <div class="flex items-center">
                      <div
                        class="h-2.5 w-2.5 rounded-full bg-red-500 me-2"
                      ></div>
                      Inactivo
                    </div>
                  </td>
                  <td class="px-6 py-3">
                    <a
                      href="#"
                      class="flex font-medium text-gray-600 hover:underline"
                    >
                      <svg
                        class="w-5 h-5 text-gray-800 dark:text-white"
                        aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg"
                        width="24"
                        height="24"
                        fill="none"
                        viewBox="0 0 24 24"
                      >
                        <path
                          stroke="currentColor"
                          stroke-linecap="square"
                          stroke-linejoin="round"
                          stroke-width="1"
                          d="M7 19H5a1 1 0 0 1-1-1v-1a3 3 0 0 1 3-3h1m4-6a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm7.441 1.559a1.907 1.907 0 0 1 0 2.698l-6.069 6.069L10 19l.674-3.372 6.07-6.07a1.907 1.907 0 0 1 2.697 0Z"
                        />
                      </svg>
                      Editar
                    </a>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { ref } from "vue";
import Modalpss from "../modalpss.vue";

// Estado para controlar la visibilidad del modal
const isModalOpen = ref(false);

// Método para abrir el modal
const openModal = () => {
  isModalOpen.value = true;
};

// Método para cerrar el modal
const closeModal = () => {
  isModalOpen.value = false;
};
</script>
