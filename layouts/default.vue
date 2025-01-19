<template>
  <div>
    <header>
      <h1>OLIVENCE</h1>
      <nav>
        <ul>
          <li><NuxtLink to="/">Главная</NuxtLink></li>
          <li><NuxtLink to="/about">Об Olivence</NuxtLink></li>
        </ul>
      </nav>
    </header>

    <main>
      <NuxtPage />
    </main>

    <footer>
      <p>&copy; 2025</p>
    </footer>
  </div>
</template>

<script setup></script>

<style>
header {
  background: var(--oliv-dark02);
  color: var(--oliv-light02);
  padding: 20px;
}

footer {
  text-align: center;
  padding: 10px;
  background: #333;
  color: var(--oliv-light02);
}

nav ul {
  list-style-type: none;
  display: flex;
  gap: 10px;
}

main {

}
</style>
