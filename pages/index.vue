<template>
  <div class="container">
     <h1 class="page-title">Formula One Driverを紹介するサイト。</h1>
    <ul>
      <li>
        <nuxt-link to="/Driver/Senna">アイルトン・セナ</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/Driver/Schumache">ミハエル・シューマッハ</nuxt-link>
      </li>
    </ul>
  </div>
  <style>
  
  .background {
  background-image: url('/Image/F1logo.jpg');
  background-size: cover;
  background-position: center;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
}
  </style>

<footer>
            <p>&copy; 2024 Formula One</p>
        </footer>
    </template>