<template>
  <footer class="bg-gray-900 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <!-- Hotel Information -->
        <div class="col-span-1 lg:col-span-2">
          <div class="flex items-center space-x-2 mb-4">
            <img src="/logo-white.png" alt="Dayan Hotel" class="h-10 w-auto" />
            <span class="text-xl font-bold text-white">
              {{ $t('common.hotel_name', 'Даян зочид буудал') }}
            </span>
          </div>
          <p class="text-gray-300 mb-6 max-w-md">
            {{ $t('home.hero_description') }}
          </p>
          
          <!-- Contact Info -->
          <div class="space-y-3">
            <div class="flex items-center space-x-3">
              <MapPinIcon class="h-5 w-5 text-accent-400" />
              <span class="text-gray-300">
                Улиастай хот, Завхан аймag, Монгол улс
              </span>
            </div>
            <div class="flex items-center space-x-3">
              <PhoneIcon class="h-5 w-5 text-accent-400" />
              <span class="text-gray-300">+976 7012-3456</span>
            </div>
            <div class="flex items-center space-x-3">
              <EnvelopeIcon class="h-5 w-5 text-accent-400" />
              <span class="text-gray-300">info@dayanhotel.mn</span>
            </div>
          </div>
        </div>

        <!-- Quick Links -->
        <div>
          <h3 class="text-lg font-semibold mb-4">{{ $t('footer.quick_links') }}</h3>
          <ul class="space-y-2">
            <li>
              <NuxtLink to="/" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.home') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/rooms" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.rooms') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/services" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.services') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/restaurant" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.restaurant') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/gallery" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.gallery') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.about') }}
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/contact" class="text-gray-300 hover:text-white transition-colors">
                {{ $t('navigation.contact') }}
              </NuxtLink>
            </li>
          </ul>
        </div>

        <!-- Services -->
        <div>
          <h3 class="text-lg font-semibold mb-4">{{ $t('navigation.services') }}</h3>
          <ul class="space-y-2">
            <li class="text-gray-300">{{ $t('services.restaurant') }}</li>
            <li class="text-gray-300">{{ $t('services.spa') }}</li>
            <li class="text-gray-300">{{ $t('services.laundry') }}</li>
            <li class="text-gray-300">{{ $t('services.transport') }}</li>
            <li class="text-gray-300">{{ $t('services.wifi') }}</li>
            <li class="text-gray-300">{{ $t('services.parking') }}</li>
            <li class="text-gray-300">{{ $t('services.conference') }}</li>
          </ul>
        </div>
      </div>

      <!-- Social Media & Newsletter -->
      <div class="border-t border-gray-800 mt-8 pt-8">
        <div class="flex flex-col md:flex-row justify-between items-center">
          <!-- Social Media -->
          <div class="flex items-center space-x-6 mb-4 md:mb-0">
            <span class="text-gray-300">{{ $t('footer.follow_us') }}:</span>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                <path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"/>
              </svg>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                <path d="M22.46 6c-.77.35-1.6.58-2.46.69.88-.53 1.56-1.37 1.88-2.38-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29 0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15 0 1.49.75 2.81 1.91 3.56-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07 4.28 4.28 0 0 0 4 2.98 8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21 16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56.84-.6 1.56-1.36 2.14-2.23z"/>
              </svg>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.174-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.741.097.118.112.223.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.402.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.357-.629-2.758-1.378l-.749 2.848c-.269 1.045-1.004 2.352-1.498 3.146 1.123.345 2.306.535 3.55.535 6.624 0 11.99-5.367 11.99-11.987C24.007 5.367 18.641.001.001 12.017z"/>
              </svg>
            </a>
          </div>

          <!-- Language Selector -->
          <div class="flex items-center space-x-4">
            <select 
              v-model="currentLocale" 
              @change="switchLanguage"
              class="bg-gray-800 text-white border border-gray-700 rounded px-3 py-1 text-sm focus:outline-none focus:border-accent-400"
            >
              <option value="mn">Монгол</option>
              <option value="en">English</option>
            </select>
          </div>
        </div>
      </div>

      <!-- Copyright -->
      <div class="border-t border-gray-800 mt-8 pt-8 text-center">
        <p class="text-gray-400 text-sm">
          {{ $t('footer.copyright') }}
        </p>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
import { 
  MapPinIcon, 
  PhoneIcon, 
  EnvelopeIcon 
} from '@heroicons/vue/24/outline'

const { $i18n } = useNuxtApp()

const currentLocale = ref($i18n.locale.value)

const switchLanguage = async () => {
  await $i18n.setLocale(currentLocale.value)
}
</script>