<script setup>
import { Alert, AlertDescription, AlertTitle } from "@/components/ui/alert";
</script>
<template>
  <main class="p-4">
    <h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">Fursona References</h1>
    <p class="leading-7 [&:not(:first-ch ild)]:mt-6">Here are some references for my fursona, Echo the Fox.</p>
    <div class="my-4">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <!-- Infobox -->
        <div class="md:col-span-1 rounded-lg shadow-md overflow-hidden border border-zinc-800">
          <div class="p-0 m-0">
            <img src="~/assets/img/art/xmr_hoodie.webp" alt="Echo the Fox" class="w-full h-auto" />
          </div>
          <div class="m-4">
            <ul>
              <li><strong>Name:</strong> Echo</li>
              <li><strong>Age:</strong> 15</li>
              <li><strong>Body Type:</strong> Anthro</li>
              <li><strong>Pronouns:</strong> he/him</li>
              <li><strong>Species:</strong> Fox</li>
              <li><strong>Gender:</strong> Male</li>
              <li><strong>Tails:</strong> 3-5</li>
            </ul>
          </div>
        </div>

        <!-- Main content -->
        <div class="md:col-span-2 space-y-6">
          <Alert class="h-full">
            <AlertTitle>About</AlertTitle>
            <AlertDescription>
              <div>Echo is an orange fox who usually wears a sweatshirt with the occasional T-shirt. Common designs include the <a class="font-semibold text-blue-500" target="_blank" href="https://web.getmonero.org/press-kit/">Monero logo</a> and the <a class="font-semibold text-blue-500" target="_blank" href="https://efimero.github.io/xenia-images/cathodegaytube1.jpg">Xenia Linux T-shirt</a>.</div>
            </AlertDescription>
            <AlertTitle class="my-2">A few notes</AlertTitle>
            <AlertDescription
              ><ul class="list-disc pl-5 space-y-1">
                <li>3 to 5 fluffy tails</li>
                <li>Orange eyes</li>
                <li>The tip of the ears are a bit darker</li>
              </ul></AlertDescription
            >
            <AlertTitle class="my-2">Do's and Don'ts</AlertTitle>
            <AlertDescription>
              <h3 class="text-xl font-semibold text-green-500">Yes!</h3>
              <ul class="list-disc pl-5 space-y-1">
                <li>Draw without asking first</li>
                <li>Pride art</li>
                <li>Design changes</li>
                <li>Body swap (humans/humanoid)</li>
              </ul>
              <h3 class="text-xl font-semibold text-red-500">No...</h3>
              <ul class="list-disc pl-5 space-y-1">
                <li>NSFW, any and all kinds</li>
                <li>Fetish/kink art</li>
                <li>Gore of any kind</li>
              </ul>
            </AlertDescription>
          </Alert>
        </div>
      </div>
    </div>
  </main>
</template>
