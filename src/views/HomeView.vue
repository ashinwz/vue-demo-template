<template>
  <div class="bg-white">
    <div class="max-w-2xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:max-w-7xl lg:px-8">
      <div class="md:flex md:items-center md:justify-between">
        <h2 class="text-2xl font-extrabold tracking-tight text-gray-900">Trending products</h2>
        <a href="#" class="hidden text-sm font-medium text-indigo-600 hover:text-indigo-500 md:block">Shop the collection<span aria-hidden="true"> &rarr;</span></a>
      </div>

      <div class="mt-6 grid grid-cols-1 gap-x-5 gap-y-10 sm:gap-x-5 md:grid-cols-2 md:gap-y-10 lg:gap-x-5">
        <div v-for="product in products" :key="product.id" class="group relative">
          <div class="grid grid-cols-2 gap-2 w-full h-56 bg-gray-200 rounded-md overflow-hidden group-hover:opacity-75 lg:h-72 xl:h-80">
            <div>
              <img :src="product.imageSrc" :alt="product.imageAlt" class="w-full h-full object-center object-cover" />
            </div>
            <div class="flex justify-center items-center">
              <img :src="product.imageSrc" :alt="product.imageAlt" class="w-3/4 h-3/4 object-center object-cover" />
            </div>

          </div>
          <h3 class="mt-4 text-sm text-gray-700">
            <a :href="product.href">
              <span class="absolute inset-0"></span>
              {{ product.name }}
            </a>
          </h3>

          <!-- Additional properties -->
          <div class="grid grid-cols-2 gap-4 w-full">
            <div>
              <div class="flex mt-1 text-sm text-gray-500">
                <div class="w-1/2">Color:</div>
                <div class="w-1/2">{{ product.color }}</div>
              </div>
              <div class="flex mt-1 text-sm font-medium text-gray-900">
                <div class="w-1/2">Price:</div>
                <div class="w-1/2">{{ product.price }}</div>
              </div>
              <div class="flex mt-1 text-sm font-medium text-gray-900">
                <div class="w-1/2">Range:</div>
                <div class="w-1/2">{{ product.range }}</div>
              </div>
            </div>
            <div>
              <div class="flex mt-1 text-sm text-gray-500">
                <div class="w-1/2">Color:</div>
                <div class="w-1/2">{{ product.color }}</div>
              </div>
              <div class="flex mt-1 text-sm font-medium text-gray-900">
                <div class="w-1/2">Price:</div>
                <div class="w-1/2">{{ product.price }}</div>
              </div>
              <div class="flex mt-1 text-sm font-medium text-gray-900">
                <div class="w-1/2">Range:</div>
                <div class="w-1/2">{{ product.range }}</div>
              </div>
            </div>
          </div>
          
        </div>
      </div>

      <div class="mt-8 text-sm md:hidden">
        <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500">Shop the collection<span aria-hidden="true"> &rarr;</span></a>
      </div>
    </div>
  </div>
</template>

<script>
const products = [
  {
    id: 1,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  {
    id: 2,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  {
    id: 3,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  {
    id: 4,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },

  {
    id: 5,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  {
    id: 6,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  {
    id: 7,
    name: 'Leather Long Wallet',
    color: 'Natural',
    price: '$75',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-04-trending-product-02.jpg',
    imageAlt: 'Hand stitched, orange leather long wallet.',
  },
  // More products...
]

export default {
  setup() {
    return {
      products,
    }
  },
}
</script>
