<template>
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayrton Senna</title>
    <style>
        /* ... 以前のスタイル ... */
        .foldable-content {
            display: none;
        }
        .foldable-header.active + .foldable-content {
            display: block;
        }
        .foldable-header {
            cursor: pointer;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>アイルトン・セナの戦績</h1>
    </header>

    <div class="container">
        <!-- プロフィール -->
        <div class="foldable">
            <div class="foldable-header">
                <h2 id="profile">プロフィール <a href="#profile">&#x1f517;</a></h2>
            </div>
            <div class="foldable-content">
                <p>
                    <!-- プロフィールの内容 -->
                </p>
            </div>
        </div>

        <!-- 主な成績 -->
        <div class="foldable">
            <div class="foldable-header">
                <h2 id="achievements">主な成績 <a href="#achievements">&#x1f517;</a></h2>
            </div>
            <div class="foldable-content">
                <ul>
                    <!-- 成績の内容 -->
                </ul>
            </div>
        </div>

        <!-- キャリアのハイライト -->
        <div class="foldable">
            <div class="foldable-header">
                <h2 id="highlights">キャリアのハイライト <a href="#highlights">&#x1f517;</a></h2>
            </div>
            <div class="foldable-content">
                <p>
                    <!-- ハイライトの内容 -->
                </p>
            </div>
        </div>

        <!-- フォーミュラ1チーム -->
        <div class="foldable">
            <div class="foldable-header">
                <h2 id="teams">フォーミュラ1チーム <a href="#teams">&#x1f517;</a></h2>
            </div>
            <div class="foldable-content">
                <p>
                    <!-- チームの内容 -->
                </p>
            </div>
        </div>

        <!-- ビデオ -->
        <div class="foldable">
            <div class="foldable-header">
                <h2 id="video">ビデオ <a href="#video">&#x1f517;</a></h2>
            </div>
            <div class="foldable-content">
                <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/nL5liGMND_0?si=KNxGl24C2rxERaZ-&amp;start=553" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2023 アイルトン・セナのファンクラブ</p>
    </footer>

    <script>
        document.querySelectorAll('.foldable-header').forEach(header => {
            header.addEventListener('click', () => {
                header.classList.toggle('active');
            });
        });
    </script>
</body>
</html>

  </template>