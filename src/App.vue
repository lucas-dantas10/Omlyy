<script setup>
// import company from "./assets/company.png";
import about from "./assets/about.svg";
import CEO from "./assets/ceo.jpg";
// import CEO from "./assets/ceo2.jpg";
</script>

<template>
    <v-app>
        <v-app-bar class="px-16" color="indigo-darken-1" flat>
            <v-app-bar-title class="font-semibold">OMLYY</v-app-bar-title>
            <v-spacer></v-spacer>
            <v-list class="flex bg-[#3949AB] text-white justify-between items-center gap-2 pr-2">
                <v-list-item href="/">
                    <v-list-item-content>
                        <v-list-item-title class="font-semibold">Home</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>

                <v-list-item href="/teste">
                    <v-list-item-content>
                        <v-list-item-title class="font-semibold">Sobre</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>

                <v-list-item href="contato">
                    <v-list-item-content>
                        <v-list-item-title class="font-semibold">Contato</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-app-bar>

        <v-main class="w-full h-full mt-8 bg-white">
            <v-container>
                <section id="home">
                    <div class="w-full h-full flex justify-between items-center">
                        <div class="h-full w-[50%] flex flex-col justify-between gap-10">
                            <h1 class="text-5xl font-bold">Premium Web Hosting for Your Website</h1>

                            <p class="text-gray-600">
                                Blazing fast web hosting for individuals and businesses of all sizes backed by
                                24x7x365 Support.
                            </p>

                            <v-btn width="50%" color="indigo-darken-1"> Fale conosco </v-btn>
                        </div>
                        <div>
                            <img :src="CEO" class="w-full shadow-2xl rounded-full" alt="Imagem da company" />
                        </div>
                    </div>
                </section>
            </v-container>

            <v-container>
                <section id="about" class="mt-28">
                    <div>
                        <h1 class="w-[120px] pb-2 text-4xl font-bold border-b-4 border-indigo-500">Sobre</h1>

                        <div class="flex items-start justify-between w-full h-full">
                            <div class="w-full">
                                <p class="mt-8 text-justify w-[80%]">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to make a type
                                    specimen book. It has survived not only five centuries, but also the leap into
                                    electronic typesetting, remaining essentially unchanged. It was popularised in
                                    the 1960s with the release of Letraset sheets containing Lorem Ipsum passages,
                                    and more recently with desktop publishing software like Aldus PageMaker
                                    including versions of Lorem Ipsum.
                                </p>
                            </div>
                            <div class="w-[80%]">
                                <img :src="about" class="w-[70%]" />
                            </div>
                        </div>
                    </div>
                </section>
            </v-container>

            <v-container class="mt-28">
                <section id="contact">
                    <h1 class="w-[150px] pb-2 text-4xl font-bold border-b-4 border-indigo-500">Contato</h1>
                    <div class="mt-6">
                        <div class="flex justify-between gap-10">
                            <form class="w-full">
                                <div class="mb-4">
                                    <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
                                        Nome
                                    </label>
                                    <input
                                        class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                                        id="name"
                                        type="text"
                                        placeholder="Nome"
                                        required
                                    />
                                </div>
                                <div class="mb-4">
                                    <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
                                        Email
                                    </label>
                                    <input
                                        class="appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                                        id="email"
                                        type="email"
                                        required
                                        placeholder="email@example.com"
                                    />
                                </div>
                                <div class="mb-4">
                                    <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
                                        Assunto
                                    </label>
                                    <textarea id="message" rows="4" class="block p-2.5 w-full text-gray-700 leading-tight rounded-lg border border-gray-300 focus:outline-none focus:shadow-outline"></textarea>

                                </div>
                                <div class="flex items-center justify-between">
                                    <button
                                        class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
                                        type="button"
                                    >
                                        Enviar
                                    </button>
                                </div>
                            </form>

                            <div class="w-full">
                                <div>
                                    <h3 class="text-2xl font-semibold">Nosso Email</h3>
                                    <p>email@example.com</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
            </v-container>
        </v-main>

        <v-footer>
            <v-container>
                <h1>FOOTER CONTENT</h1>
            </v-container>
        </v-footer>
    </v-app>
</template>
