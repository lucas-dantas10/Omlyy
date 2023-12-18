<script setup>
// import company from "./assets/company.png";
import about from "./assets/about.svg";
// import CEO from "./assets/ceo.jpg";
import CEO from "./assets/ceo2.jpg";
</script>

<template>
    <v-app>
        <v-app-bar class="px-16" color="#FFF" flat>
            <v-app-bar-title>OMLYY</v-app-bar-title>
            <v-spacer></v-spacer>
            <v-list class="flex justify-between items-center gap-2 pr-2">
                <v-list-item href="/">
                    <v-list-item-content>
                        <v-list-item-title>Home</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>

                <v-list-item href="/teste">
                    <v-list-item-content>
                        <v-list-item-title>Sobre</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>

                <v-list-item href="/teste">
                    <v-list-item-content>
                        <v-list-item-title>Contato</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-app-bar>

        <v-main class="w-full h-full mt-8 bg-white">
            <v-container>
                <section id="home">
                    <div class="w-full h-full flex justify-center gap-4">
                        <div class="w-[50%] flex flex-col gap-10">
                            <h1 class="text-6xl font-bold">Premium Web Hosting for Your Website</h1>

                            <p class="text-gray-600">
                                Blazing fast web hosting for individuals and businesses of all sizes backed by
                                24x7x365 Support.
                            </p>

                            <v-btn width="50%" color="indigo-lighten-1"> Fale conosco </v-btn>
                        </div>
                        <div>
                            <img :src="CEO" class="w-full shadow-2xl" alt="Imagem da company" />
                        </div>
                    </div>
                </section>
            </v-container>

            <v-container>
                <section id="about" class="mt-20">
                    <div>
                        <h1 class="w-[200px] pb-2 text-4xl font-bold border-b-4 border-indigo-500">Sobre Nós</h1>

                        <div class="flex gap-10 items-start justify-between w-full h-full">
                            <div class="w-[50%]">
                                <p class="mt-8 text-justify">
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
                            <div class="w-[50%]">
                                <img :src="about" class="w-[70%]" />
                            </div>
                        </div>
                    </div>
                </section>
            </v-container>
        </v-main>

        <v-footer>
            <h1>Footer Content</h1>
        </v-footer>
    </v-app>
</template>
