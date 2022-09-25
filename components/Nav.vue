<template>
  <nav class="navbar navbar-expand-lg sticky-top navbar-light bg-white">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div
        class="collapse navbar-collapse justify-content-center"
        id="navbarSupportedContent"
      >
        <div class="navbar-nav">
          <NuxtLink to="/" class="n-link-base nav-link"> Accueil </NuxtLink>

          <NuxtLink to="/presentation" class="n-link-base nav-link">
            Présentation
          </NuxtLink>
          <NuxtLink to="/courstarifs" class="n-link-base nav-link"
            >Cours et Tarifs
          </NuxtLink>
          <NuxtLink to="/professeurs" class="n-link-base nav-link">
            Professeurs
          </NuxtLink>
          <NuxtLink to="/inscriptions" class="n-link-base nav-link">
            Inscriptions
          </NuxtLink>
          <NuxtLink to="/informationsgenerales" class="n-link-base nav-link">
            Informations Générales
          </NuxtLink>
          <NuxtLink to="/planacces" class="n-link-base nav-link">
            Plan d'accès
          </NuxtLink>
          <NuxtLink to="/seminaires" class="n-link-base nav-link">
            Séminaires
          </NuxtLink>
        </div>
        <!-- <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="/">Accueil</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/presentation">Présentation</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/coursettarifs">Cours et Tarifs</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/professeurs">Professeurs</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/inscription">Inscription</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/informationsgenerales"
              >Informations Générales</a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/plandacces">Plan d'accès</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/seminaires">Nos séminaires</a>
          </li>
        </ul> -->
      </div>
    </div>
  </nav>
</template>