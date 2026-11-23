---
theme: default
title: De idea a internet
colorSchema: light
transition: fade
fonts:
  sans: Inter
  mono: JetBrains Mono
---

<div class="center-stack">
  <div class="row gap-14 text-8xl">
    <ph-laptop-duotone v-motion :initial="{ y: 40, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 0 } }" />
    <ph-arrow-right-bold class="muted text-5xl" v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 300 } }" />
    <ph-globe-hemisphere-west-duotone class="accent" v-motion :initial="{ y: 40, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 600 } }" />
  </div>
  <h1 class="mt-14">De idea a internet</h1>
  <p class="muted">Hackathon Codex</p>
</div>

<!--
Bienvenida. Objetivo de estos 5 minutos: que todo el mundo entienda las 3 piezas
que hacen falta para que lo que construyáis hoy lo pueda abrir cualquiera desde su móvil.
-->

---

<div class="center-stack">
  <div class="row gap-24">
    <div class="piece" v-click>
      <logos-github-icon class="text-8xl" />
      <span>Código</span>
    </div>
    <div class="piece" v-click>
      <logos-vercel-icon class="text-8xl" />
      <span>Servidor</span>
    </div>
    <div class="piece" v-click>
      <ph-signpost-duotone class="text-8xl accent" />
      <span>Dirección</span>
    </div>
  </div>
</div>

<!--
Tres piezas, tres cosas distintas. La gente las mezcla todo el rato.
[click] Dónde se GUARDA el código.
[click] Dónde se EJECUTA para que otros lo vean.
[click] Cómo te ENCUENTRAN.
Analogía que vamos a usar: un restaurante. Receta, cocina, dirección.
-->

---

<div class="center-stack">
  <div class="row gap-10">
    <ph-laptop-duotone class="text-9xl" />
    <div class="flow-arrow" v-click>
      <code>git push</code>
      <ph-arrow-right-bold class="text-4xl muted" />
    </div>
    <logos-github-icon class="text-9xl" v-click="1" />
  </div>

  <h2 class="mt-14">GitHub: donde <em>vive</em> el código</h2>

  <div class="row gap-16 mt-10 text-4xl muted">
    <div class="chip" v-click><ph-clock-counter-clockwise-duotone /> historial</div>
    <div class="chip" v-click><ph-shield-check-duotone /> copia segura</div>
    <div class="chip" v-click><ph-users-three-duotone /> en equipo</div>
  </div>
</div>

<!--
GitHub es el RECETARIO. Guarda la receta (el código), pero aquí no se cocina nada.
- Cada cambio queda guardado: puedes volver atrás si Codex rompe algo.
- Si se te muere el portátil, el código sigue ahí.
- Tus compañeros de equipo trabajan sobre el mismo código.
Importante: tener el código en GitHub NO significa que la web esté online.
-->

---

<div class="center-stack">
  <div class="row gap-10 text-7xl">
    <logos-github-icon class="text-8xl" />
    <ph-arrow-right-bold class="text-4xl muted" />
    <logos-vercel-icon class="text-8xl" v-click />
    <ph-arrow-right-bold class="text-4xl muted" v-click />
    <ph-globe-hemisphere-west-duotone class="accent text-8xl" v-click="'+0'" />
  </div>

  <h2 class="mt-14">Desplegar: donde <em>corre</em> el código</h2>

  <div class="url mt-8" v-click>https://mi-app.vercel.app</div>

  <div class="row gap-8 mt-12 text-3xl faint" v-click>
    <logos-netlify-icon /> <logos-cloudflare-icon /> <logos-railway />
  </div>
</div>

<!--
Desplegar = abrir la COCINA al público. Un ordenador encendido 24/7 que sirve tu web.
[click] Vercel se conecta a tu GitHub. Cada vez que haces push, publica la nueva versión solo.
[click] Y te da una URL gratis al momento.
[click] Hay alternativas (Netlify, Cloudflare, Railway); hoy usamos Vercel porque es lo más rápido.
GitHub guarda. Vercel sirve.
-->

---

<div class="center-stack">
  <div class="row gap-8">
    <div class="url" v-mark.strike-through.red="1">mi-app.vercel.app</div>
    <ph-arrow-right-bold class="text-4xl muted" v-click="1" />
    <div class="url big accent-bg" v-click="1">miapp.com</div>
  </div>

  <h2 class="mt-12">El dominio: tu <em>dirección</em></h2>

  <div class="row gap-6 mt-10 text-3xl muted" v-click>
    <span class="mono">miapp.com</span>
    <ph-arrow-right-bold />
    <ph-address-book-duotone class="text-5xl" />
    <ph-arrow-right-bold />
    <logos-vercel-icon />
  </div>

  <div class="row gap-12 mt-12 text-3xl" v-click>
    <div class="chip"><ph-coins-duotone /> ~10 €/año</div>
    <div class="chip"><ph-shopping-cart-duotone /> se alquila, no se compra para siempre</div>
  </div>
</div>

<!--
El dominio es la DIRECCIÓN del restaurante. La cocina ya existe, pero nadie recuerda "mi-app.vercel.app".
[click] Compras un nombre corto y tuyo.
[click] Cómo funciona: el DNS es la agenda de contactos de internet. Traduce el nombre a la dirección
del servidor (Vercel). Tú solo apuntas el dominio a Vercel y listo.
[click] Se alquila por años (~10 €), en Namecheap, Cloudflare o el propio Vercel.
Para hoy NO hace falta: la URL gratis de Vercel es suficiente. Es para cuando el proyecto sea en serio.
-->

---

<div class="center-stack">
  <div class="row gap-6 text-6xl">
    <ph-laptop-duotone v-click />
    <ph-arrow-right-bold class="text-3xl muted" v-click="1" />
    <logos-github-icon v-click />
    <ph-arrow-right-bold class="text-3xl muted" v-click="2" />
    <logos-vercel-icon v-click />
    <ph-arrow-right-bold class="text-3xl muted" v-click="3" />
    <span class="url small" v-click>miapp.com</span>
    <ph-arrow-right-bold class="text-3xl muted" v-click="4" />
    <ph-users-three-duotone class="accent" v-click />
  </div>

  <h1 class="mt-16" v-click>¡A construir!</h1>
</div>

<!--
Todo junto. Escribes con Codex en tu portátil → push a GitHub → Vercel lo publica solo
→ el dominio lleva a la gente hasta ahí → la gente lo usa.
Primer objetivo del día: tener un "hola mundo" online en la primera hora. Luego, a iterar.
-->
