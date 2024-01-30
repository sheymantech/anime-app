<script setup></script>

<template>
  <div class="container">
    <div class="anime-app">
      <header>
        <h1 class="text-center">THE<strong>ANIME</strong>APP</h1>
      </header>
      <form>
        <input type="search" placeholder="search for an anime...." />
      </form>
      <div class="row">
        <div class="col-md-4">
          <img
            src="https://placehold.it/154x250"
            alt="Anime poster"
            class="anime-img"
          />
          <h3>Naruto</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.anime-app {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 4rem 0;
  flex-direction: column;

  h1 {
    color: rgb(80, 78, 78);
    word-spacing: 2px;
    strong {
      color: black;
    }
  }

  form {
    display: block;
    margin: 2rem 6rem;
    width: 100%;

    input {
      width: 100%;
      outline: none;
      border: none;
      appearance: none;
      background-color: rgb(245, 239, 239);
      padding: 0.9rem;
      border-radius: 8px;
      box-shadow: 0 0 8px 2px rgb(199, 192, 192);
    }

    input:focus {
      background-color: black;
      color: white;
    }
  }
  .anime-img {
    border-radius: 16px;
    height: 300px;
    object-fit: cover;
    box-shadow: 0 0 8px 2px rgb(0, 0, 0, 0.15);
    transition: 0.4s;
  }
  .anime-img:hover {
    transform: scale(1.04);
  }
  h3 {
    font-size: 19px;
    font-weight: 900;
  }
}
</style>
