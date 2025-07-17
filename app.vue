<template>
    <div
        class="md:min-h-screen bg-gradient-to-br from-[#000000] via-[#060026] to-[#180385] flex flex-col items-center justify-center">
        <div
            class="absolute md:top-14 top-6 right-6 md:right-40 flex items-center space-x-2 text-white font-medium xs:hidden">
            <div class="w-6 h-6 rounded-full overflow-hidden">
                <img src="https://flagcdn.com/w80/gb.png" alt="UK Flag" class="w-full h-full object-cover" />
            </div>
            <span class="text-sm">English</span>
            <img src="/public/images/vector.png" alt="24markets.com" />
        </div>

        <div class="md:py-10 py-4">
            <img src="/public/images/logo.png" alt="24markets.com" class="h-12" />
        </div>

        <div class="flex flex-col gap-8 w-full max-w-3xl px-4">
            <div class="w-full border border-white/20 rounded-2xl">
                <div class="md:flex">
                    <div>
                        <div
                            class="md:w-[20rem] md:h-full h-[20rem] bg-white rounded-2xl flex items-center justify-center">
                            <div class="text-center">
                                <p>Image Placeholder</p>
                            </div>
                        </div>
                    </div>
                    <div class="bg-[#0e0352]/40 backdrop-blur-lg rounded-2xl md:px-8 px-4">

                        <div class="w-full">

                            <h2 class=" text-gray-400 text-xl font-semibold py-6 text-center">Join us today x reason!
                            </h2>

                            <div class="space-y-4">
                                <div class="relative">
                                    <div class="absolute left-3 top-3 ">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20"
                                            fill="currentColor">
                                            <path
                                                d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
                                            <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
                                        </svg>
                                    </div>
                                    <input type="email" placeholder="Email Address"
                                        class="w-full bg-white rounded-full py-3 pl-10 pr-6 text-gray-900 placeholder-gray-500 focus:outline-none focus:ring-2 focus:ring-[#190292]" />
                                    <div class="absolute right-3 top-3">
                                        <img src="/public/images/check.png" alt="24markets.com" />
                                    </div>
                                </div>

                                <div class="relative">
                                    <div class="absolute left-3 top-3 ">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20"
                                            fill="currentColor">
                                            <path fill-rule="evenodd"
                                                d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
                                                clip-rule="evenodd" />
                                        </svg>
                                    </div>

                                    <input :type="showPassword ? 'text' : 'password'" placeholder="Password"
                                        class="w-full bg-white rounded-full py-3 pl-10 pr-6 text-gray-900 placeholder-gray-500 focus:outline-none focus:ring-2 focus:ring-[#190292]" />

                                    <button class="absolute right-3 top-3 " @click="togglePasswordVisibility">
                                        <svg v-if="!showPassword" xmlns="http://www.w3.org/2000/svg" class="h-5 w-5"
                                            viewBox="0 0 20 20" fill="currentColor">
                                            <path d="M10 12a2 2 0 100-4 2 2 0 000 4z" />
                                            <path fill-rule="evenodd"
                                                d="M.458 10C1.732 5.943 5.522 3 10 3s8.268 2.943 9.542 7c-1.274 4.057-5.064 7-9.542 7S1.732 14.057.458 10zM14 10a4 4 0 11-8 0 4 4 0 018 0z"
                                                clip-rule="evenodd" />
                                        </svg>

                                        <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-5 w-5"
                                            viewBox="0 0 20 20" fill="currentColor">
                                            <path fill-rule="evenodd"
                                                d="M3.707 2.293a1 1 0 00-1.414 1.414l14 14a1 1 0 001.414-1.414l-1.473-1.473A10.014 10.014 0 0019.542 10C18.268 5.943 14.478 3 10 3a9.958 9.958 0 00-4.512 1.074l-1.78-1.781zm4.261 4.26l1.514 1.515a2.003 2.003 0 012.45 2.45l1.514 1.514a4 4 0 00-5.478-5.478z"
                                                clip-rule="evenodd" />
                                            <path
                                                d="M12.454 16.697L9.75 13.992a4 4 0 01-3.742-3.741L2.335 6.578A9.98 9.98 0 00.458 10c1.274 4.057 5.065 7 9.542 7 .847 0 1.669-.105 2.454-.303z" />
                                        </svg>

                                    </button>
                                </div>
                            </div>
                        </div>

                        <div class="w-full flex items-center justify-center">

                            <button
                                class="w-1/2 bg-white rounded-full py-3 px-6 mt-6 font-medium hover:opacity-90 transition-opacity flex items-center justify-center gap-2">
                                <span class="font-medium text-[#120083]">
                                    Register
                                </span>

                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-[#120083]"
                                    viewBox="0 0 20 20" fill="currentColor">
                                    <path fill-rule="evenodd"
                                        d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                        clip-rule="evenodd" />
                                </svg>

                            </button>
                        </div>

                        <div class="mt-6">
                            <p class="text-gray-400 text-center text-sm font-semibold mb-6">Or continue with:</p>
                            <div class="flex justify-center gap-3">
                                <button class="w-12 h-8 bg-[#1877F2] rounded-xl flex items-center justify-center">
                                    <svg class="w-4 h-4 text-white" viewBox="0 0 24 24" fill="currentColor">
                                        <path
                                            d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z" />
                                    </svg>
                                </button>

                                <button class="w-12 h-8 bg-white rounded-xl flex items-center justify-center">
                                    <svg class="w-4 h-4" viewBox="0 0 24 24">
                                        <path fill="#EA4335"
                                            d="M5.266 9.765A7.077 7.077 0 0 1 12 4.909c1.69 0 3.218.6 4.418 1.582L19.91 3C17.782 1.145 15.055 0 12 0 7.27 0 3.198 2.698 1.24 6.65l4.026 3.115Z" />
                                        <path fill="#34A853"
                                            d="M16.04 18.013c-1.09.703-2.474 1.078-4.04 1.078a7.077 7.077 0 0 1-6.723-4.823l-4.04 3.067A11.965 11.965 0 0 0 12 24c2.933 0 5.735-1.043 7.834-3l-3.793-2.987Z" />
                                        <path fill="#4A90E2"
                                            d="M19.834 21c2.195-2.048 3.62-5.096 3.62-9 0-.71-.109-1.473-.272-2.182H12v4.637h6.436c-.317 1.559-1.17 2.766-2.395 3.558L19.834 21Z" />
                                        <path fill="#FBBC05"
                                            d="M5.277 14.268A7.12 7.12 0 0 1 4.909 12c0-.782.125-1.533.357-2.235L1.24 6.65A11.934 11.934 0 0 0 0 12c0 1.92.445 3.73 1.237 5.335l4.04-3.067Z" />
                                    </svg>
                                </button>

                                <button class="w-12 h-8 bg-black rounded-xl flex items-center justify-center">
                                    <svg class="w-4 h-4 text-white" viewBox="0 0 24 24" fill="currentColor">
                                        <path
                                            d="M12.152 6.896c-.948 0-2.415-1.078-3.96-1.04-2.04.027-3.91 1.183-4.961 3.014-2.117 3.675-.546 9.103 1.519 12.09 1.013 1.454 2.208 3.09 3.792 3.039 1.52-.065 2.09-.987 3.935-.987 1.831 0 2.35.987 3.96.948 1.637-.026 2.676-1.48 3.676-2.948 1.156-1.688 1.636-3.325 1.662-3.415-.039-.013-3.182-1.221-3.22-4.857-.026-3.04 2.48-4.494 2.597-4.559-1.429-2.09-3.623-2.324-4.39-2.376-2-.156-3.675 1.09-4.61 1.09zM15.53 3.83c.843-1.012 1.4-2.427 1.245-3.83-1.207.052-2.662.805-3.532 1.818-.78.896-1.454 2.338-1.273 3.714 1.338.104 2.715-.688 3.559-1.701" />
                                    </svg>
                                </button>
                            </div>
                        </div>

                        <div class="py-6 text-gray-400 text-xs text-center font-semibold">
                            <span>By creating an account, I confirm that I have read and understood the</span>
                            <a href="#" class="text-white pl-1">Privacy Policy</a>
                        </div>

                    </div>
                </div>
            </div>

            <div class="w-full border border-white/20 rounded-2xl mb-6">
                <div class="bg-[#0e0352]/40 backdrop-blur-lg rounded-2xl p-4">
                    <div class="text-center">
                        <p class="text-white flex items-center justify-center gap-6">
                            Already have an account?
                            <button
                                class="border border-white/20 rounded-2xl px-6 py-2 hover:bg-white/5 transition-all  flex items-center justify-center gap-2">
                                <span class="text-white font-bold">
                                    Login
                                </span>
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" viewBox="0 0 20 20"
                                    fill="currentColor">
                                    <path fill-rule="evenodd"
                                        d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                        clip-rule="evenodd" />
                                </svg>
                            </button>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const showPassword = ref(false)
const togglePasswordVisibility = () => {
    showPassword.value = !showPassword.value
}
</script>