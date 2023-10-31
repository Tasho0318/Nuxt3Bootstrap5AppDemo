<template>
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1.0"
    />
    <title>トレーニングサイト</title>
  </head>
  <body>
    <div id="app">
      <header>
        <h1>トレーニングサイト</h1>
        <nav>
          <ul>
            <li><a href="#">ホーム</a></li>
            <li><a href="#">トレーニングプラン</a></li>
            <li><a href="#">コンタクト</a></li>
          </ul>
        </nav>
      </header>
      <section class="main-content">
        <h2>ようこそ、トレーニングサイトへ</h2>
        <p>
          {{ welcomeMessage }}
        </p>
      </section>
      <section class="training-plans">
        <h2>トレーニングプラン</h2>
        <ul>
          <li v-for="plan in trainingPlans" :key="plan">{{ plan }}</li>
        </ul>
      </section>
      <footer>
        <p>&copy; 2023 トレーニングサイト</p>
      </footer>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/vue@2.6.14/dist/vue.js"></script>
    <script>
      new Vue({
        el: "#app",
        data: {
          welcomeMessage:
            "私たちのウェブサイトでは、健康的な生活とフィットネスに関する情報を提供しています。トレーニングプラン、栄養情報、健康のヒントなどを見つけてください。",
          trainingPlans: [
            "初心者向けトレーニング",
            "筋力トレーニング",
            "有酸素運動",
          ],
        },
      });
    </script>
  </body>
</html>
</template>