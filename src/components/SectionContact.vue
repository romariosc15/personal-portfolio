<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faLocationDot, faEnvelope } from '@fortawesome/free-solid-svg-icons'
import { faLinkedinIn } from '@fortawesome/free-brands-svg-icons'
</script>

<template>
  <section class="bg-black">
    <div class="container mx-auto py-16 px-16">
      <div class="grid grid-cols-2 gap-24">
        <div class="bg-[#15091d] rounded-xl px-12 py-16">
          <h2 class="text-4xl font-semibold text-violet-400 mb-4">
            Let&apos;s collaborate
          </h2>
          <p class="text-base font-light text-white mb-8">
            Let&apos;s talk and bring your idea to life
          </p>
          <form class="space-y-4" action="">
            <div class="grid grid-cols-2 gap-4">
              <input
                class="bg-[#050709] border border-[#22272c] rounded-lg text-white py-3 px-5"
                type="text"
                placeholder="First name"
                name=""
                id=""
                required
              />
              <input
                class="bg-[#050709] border border-[#22272c] rounded-lg text-white py-3 px-5"
                type="text"
                placeholder="Last name"
                name=""
                id=""
              />
            </div>
            <div class="grid grid-cols-2 gap-4">
              <input
                class="bg-[#050709] border border-[#22272c] rounded-lg text-white py-3 px-5"
                type="email"
                placeholder="Email address"
                name=""
                id=""
                required
              />
            </div>
            <div>
              <input
                class="bg-[#050709] border border-[#22272c] rounded-lg text-white py-3 px-5 w-full"
                type="text"
                placeholder="Subject"
                name=""
                id=""
                required
              />
            </div>
            <div>
              <textarea
                class="bg-[#050709] border border-[#22272c] rounded-lg text-white py-3 px-5 w-full"
                placeholder="Message"
                name=""
                id=""
                rows="5"
                required
              ></textarea>
            </div>
            <div>
              <button
                class="transition-colors px-8 py-3 font-semibold rounded-full border text-white border-violet-600 bg-violet-600 hover:bg-violet-800 hover:border-violet-800"
                type="submit"
              >
                Send message
              </button>
            </div>
          </form>
        </div>
        <div class="space-y-8 content-center">
          <div class="text-white flex flex-row gap-8 items-center">
            <div
              class="bg-violet-700 rounded-full content-center text-center w-12 h-12"
            >
              <FontAwesomeIcon
                class="w-6 h-6 align-middle text-gray-300"
                :icon="faEnvelope"
              />
            </div>
            <div class="space-y-1">
              <p class="text-gray-300">Email</p>
              <a
                class="transition-colors inline-block text-xl font-medium text-white hover:text-violet-500"
                href="mailto:romariosc15@outlook.com"
              >
                romariosc15@outlook.com
              </a>
            </div>
          </div>
          <div class="text-white flex flex-row gap-8 items-center">
            <div
              class="bg-violet-700 rounded-full content-center text-center w-12 h-12"
            >
              <FontAwesomeIcon
                class="w-6 h-6 align-middle text-gray-300"
                :icon="faLinkedinIn"
              />
            </div>
            <div class="space-y-1">
              <p class="text-gray-300">LinkedIn</p>
              <a
                class="transition-colors inline-block text-xl font-medium text-white hover:text-violet-500"
                href="https://www.linkedin.com/in/romariosarmiento"
                target="_blank"
              >
                /in/romariosarmiento
              </a>
            </div>
          </div>
          <div class="text-white flex flex-row gap-8 items-center">
            <div
              class="bg-violet-700 rounded-full content-center text-center w-12 h-12"
            >
              <FontAwesomeIcon
                class="w-6 h-6 align-middle text-gray-300"
                :icon="faLocationDot"
              />
            </div>
            <div class="space-y-1">
              <p class="text-gray-300">Location</p>
              <p class="text-xl font-medium">Ilo, Moquegua</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
