<template>
  <div class="bg-white py-24 sm:py-32 lg:py-20">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="sm:text-center">
        <h2 class="text-lg font-semibold leading-8 text-orange-600">Henoo</h2>
        <p
          class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl"
        >
          Test technique dev front web
        </p>
        <p class="mx-auto mt-6 max-w-2xl text-lg leading-8 text-gray-600">
          Bienvenue dans ce technique conçut par l'équipe technique d'Henoo !
        </p>
        <p class="mx-auto mt-6 max-w-2xl text-lg leading-5 text-gray-600">
          Le but de ce test est d'évaluer tes compétences sur des
          technologies web que nous utilisons pour nos projets. Le principe va
          être de créer une page en reproduisant le plus fidèlement possible une
          maquette donnée. <br />
          <br />
          Nous allons nous intéresser à l'aspect esthétique et design de la page
          il n'est donc pas nécessaire d'implémenter le côté "fonctionnel" des
          boutons et menus mais si tu souhaites nous montrer tes talents de
          développeur et ajouter des fonctionnalités à ta création fais toi
          plaisir !
          <br />
          <br />
          Comme tu pourras le remarquer la maquette fournie représente l'état
          d'une page d'application web sur un écran large. Ta version développée
          devra être utilisable sur un smartphone. A toi de développer les
          qualités responsives de cet écran.
        </p>
      </div>

      <div class="mt-20 max-w-lg sm:mx-auto md:max-w-none">
        <div
          class="grid grid-cols-1 gap-y-16 md:grid-cols-2 md:gap-x-12 md:gap-y-16"
        >
          <div
            v-for="feature in features"
            :key="feature.name"
            class="relative flex flex-col gap-6 sm:flex-row md:flex-col lg:flex-row"
          >
            <div
              class="flex h-12 w-12 items-center justify-center rounded-xl bg-orange-500 text-white sm:shrink-0"
            ></div>
            <div class="sm:min-w-0 sm:flex-1">
              <p class="text-lg font-semibold leading-8 text-gray-900">
                {{ feature.name }}
              </p>
              <p class="mt-2 text-base leading-7 text-gray-600">
                {{ feature.description }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const features = [
  {
    name: "Début du projet",
    description:
      "Clone ce dépôt github et héberge le sur ton compte github personnel tu vas pouvoir réaliser l'exercice en partant de ce projet. Crée une nouvelle page pour réaliser la maquette et ajoute à cette page d'accueil existante un button de redirection vers ta page à toi.",
  },
  {
    name: "Condition minimales",
    description:
      'Pour exécuter ce projet tu auras besoin de node.js version 18 (ou supérieures) et de git. Pour ce qui est de la maquette tu l\'as trouvera dans le dossier "assets" de ce dépôt.',
  },
  {
    name: "Technologies utilisées",
    description:
      "Les technologies utilisées dans ce projet et que tu dois utiliser sont les suivantes : vue.js 3 (https://vuejs.org/) - nuxt js 3 (https://nuxt.com/) - tailwindcss (https://tailwindcss.com/)",
  },
  {
    name: "Fin du test",
    description:
      "Lorsque tu as fini penses à bien commit tout tes changements sur ton dépot personnel puis envoi nous par email le liens vers ce dépot.",
  },
];
</script>
