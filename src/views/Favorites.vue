<template>
  <div class="overflow-y-hidden">
    <div
      class="mx-auto container px-4 md:px-6 2xl:px-0 py-12 flex justify-center items-center"
    >
      <div class="flex flex-col jusitfy-start items-start">
        <div>
          <p class="text-sm leading-4 text-gray-600">Home</p>
        </div>
        <div class="mt-3">
          <h1
            class="text-3xl lg:text-4xl tracking-tight font-semibold leading-8 lg:leading-9 text-gray-800"
          >
            Favourites
          </h1>
        </div>
        <div class="mt-8">
          <p class="text-2xl tracking-tight leading-6 text-gray-600">
            03 items
          </p>
        </div>
        <div
          class="mt-10 lg:mt-12 grid grid-cols-1 lg:grid-cols-3 gap-x-8 gap-y-10 lg:gap-y-0"
        >
          <div class="flex flex-col">
            <div class="relative">
              <img
                class="hidden lg:block rounded-xl w-64"
                src="https://images.unsplash.com/photo-1611312449408-fcece27cdbb7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NzJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="bag"
              />
              <img
                class="hidden sm:block rounded-xl lg:hidden w-64"
                src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NjN8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="bag"
              />
              <img
                class="sm:hidden rounded-xl w-64"
                src="https://images.unsplash.com/photo-1551232864-3f0890e580d9?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="bag"
              />
              <button
                aria-label="close"
                class="top-4 right-4 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 absolute p-1.5 bg-gray-800 text-white hover:text-gray-400"
              >
                <svg
                  class="fil-current"
                  width="14"
                  height="14"
                  viewBox="0 0 14 14"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M13 1L1 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M1 1L13 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
            <div class="mt-6 flex justify-between items-center">
              <div class="flex justify-center items-center">
                <p
                  class="tracking-tight text-2xl font-semibold leading-6 text-gray-800"
                >
                  New York Streak
                </p>
              </div>
              <div class="flex justify-center items-center">
                <button
                  aria-label="show menu"
                  @click="show = !show"
                  class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 py-2.5 px-2 bg-gray-800 text-white hover:text-gray-400"
                >
                  <svg
                    v-if="show"
                    id="chevronUp1"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M9 5L5 1L1 5"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                  <svg
                    id="chevronDown1"
                    v-if="!show"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1 1L5 5L9 1"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div
              v-if="show"
              id="menu1"
              class="flex flex-col jusitfy-start items-start mt-12"
            >
              <div>
                <p class="tracking-tight text-xs leading-3 text-gray-800">
                  MK617
                </p>
              </div>
              <div class="mt-2">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  Beige brown
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  42 size
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  $1,000
                </p>
              </div>
              <div
                class="flex jusitfy-between flex-col lg:flex-row items-center mt-10 w-full space-y-4 lg:space-y-0 lg:space-x-4 xl:space-x-8"
              >
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-gray-800 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-gray-300 hover:text-gray-800 bg-white border border-gray-800"
                  >
                    More information
                  </button>
                </div>
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-black bg-gray-800 border border-gray-800"
                  >
                    Add to cart
                  </button>
                </div>
              </div>
            </div>
          </div>

          <div class="flex flex-col">
            <div class="relative">
              <img
                class="hidden lg:block rounded-xl w-64"
                src="https://images.unsplash.com/photo-1551232864-3f0890e580d9?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="watch"
              />
              <img
                class="hidden sm:block lg:hidden rounded-xl w-64"
                src="https://images.unsplash.com/photo-1611312449408-fcece27cdbb7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NzJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="watch"
              />
              <img
                class="sm:hidden rounded-xl w-64"
                src="https://images.unsplash.com/photo-1551232864-3f0890e580d9?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="watch"
              />
              <button
                aria-label="close"
                class="top-4 right-4 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 absolute p-1.5 bg-gray-800 text-white hover:text-gray-400"
              >
                <svg
                  class="fil-current"
                  width="14"
                  height="14"
                  viewBox="0 0 14 14"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M13 1L1 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M1 1L13 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
            <div class="mt-6 flex justify-between items-center">
              <div class="flex justify-center items-center">
                <p
                  class="tracking-tight text-2xl font-semibold leading-6 text-gray-800"
                >
                  Luxe 3 series
                </p>
              </div>
              <div class="flex justify-center items-center">
                <button
                  aria-label="show menu"
                  @click="show1 = !show1"
                  class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 py-2.5 px-2 bg-gray-800 text-white hover:text-gray-400"
                >
                  <svg
                    id="chevronUp2"
                    v-if="show1"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M9 5L5 1L1 5"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                  <svg
                    id="chevronDown2"
                    v-if="!show1"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1 1L5 5L9 1"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div
              id="menu2"
              v-if="show1"
              class="flex flex-col jusitfy-start items-start mt-12"
            >
              <div>
                <p class="tracking-tight text-xs leading-3 text-gray-800">
                  MK617
                </p>
              </div>
              <div class="mt-2">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  Beige brown
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  42 size
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  $1,000
                </p>
              </div>
              <div
                class="flex jusitfy-between flex-col lg:flex-row items-center mt-10 w-full space-y-4 lg:space-y-0 lg:space-x-4 xl:space-x-8"
              >
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-gray-800 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-gray-300 hover:text-gray-800 bg-white border border-gray-800"
                  >
                    More information
                  </button>
                </div>
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-black bg-gray-800 border border-gray-800"
                  >
                    Add to cart
                  </button>
                </div>
              </div>
            </div>
          </div>

          <div class="flex flex-col">
            <div class="relative">
              <img
                class="hidden lg:block rounded-xl w-64"
                src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NjN8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="shoes"
              />
              <img
                class="hidden sm:block lg:hidden rounded-xl w-64"
                src="https://images.unsplash.com/photo-1611312449408-fcece27cdbb7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NzJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="shoes"
              />
              <img
                class="sm:hidden rounded-xl w-64"
                src="https://images.unsplash.com/photo-1551232864-3f0890e580d9?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDJ8fGNsb3RoZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
                alt="shoes"
              />
              <button
                aria-label="close"
                class="top-4 right-4 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 absolute p-1.5 bg-gray-800 text-white hover:text-gray-400"
              >
                <svg
                  class="fil-current"
                  width="14"
                  height="14"
                  viewBox="0 0 14 14"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M13 1L1 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M1 1L13 13"
                    stroke="currentColor"
                    stroke-width="1.25"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
            <div class="mt-6 flex justify-between items-center">
              <div class="flex justify-center items-center">
                <p
                  class="tracking-tight text-2xl font-semibold leading-6 text-gray-800"
                >
                  EZ sneakers
                </p>
              </div>
              <div class="flex justify-center items-center">
                <button
                  aria-label="show menu"
                  @click="show2 = !show2"
                  class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 py-2.5 px-2 bg-gray-800 text-white hover:text-gray-400"
                >
                  <svg
                    id="chevronUp3"
                    v-if="show2"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M9 5L5 1L1 5"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                  <svg
                    id="chevronDown3"
                    v-if="!show2"
                    class="fill-stroke"
                    width="10"
                    height="6"
                    viewBox="0 0 10 6"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1 1L5 5L9 1"
                      stroke="currentColor"
                      stroke-width="1.25"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div
              id="menu3"
              v-if="show2"
              class="flex flex-col jusitfy-start items-start mt-12"
            >
              <div>
                <p class="tracking-tight text-xs leading-3 text-gray-800">
                  MK617
                </p>
              </div>
              <div class="mt-2">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  Beige brown
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  42 size
                </p>
              </div>
              <div class="mt-6">
                <p
                  class="tracking-tight text-base font-medium leading-4 text-gray-800"
                >
                  $1,000
                </p>
              </div>
              <div
                class="flex jusitfy-between flex-col lg:flex-row items-center mt-10 w-full space-y-4 lg:space-y-0 lg:space-x-4 xl:space-x-8"
              >
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-gray-800 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-gray-300 hover:text-gray-800 bg-white border border-gray-800"
                  >
                    More information
                  </button>
                </div>
                <div class="w-full">
                  <button
                    class="focus:outline-none focus:ring-gray-800 focus:ring-offset-2 focus:ring-2 text-white w-full tracking-tight py-4 text-lg leading-4 hover:bg-black bg-gray-800 border border-gray-800"
                  >
                    Add to cart
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Favorites",
  data() {
    return {
      show: true,
      show1: false,
      show2: false,
    };
  },
  methods: {},
  mounted() {},
};
</script>

<style></style>
