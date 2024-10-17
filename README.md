<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>动画角色信息</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            height: 100vh;
            background-image: url('熊出没.png');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            opacity: 0.9;
        }

        h1 {
            color: gold;
            font-size: 7em;
            font-family: "楷体";
            justify-content: center;
            align-items: center;
            font-weight: bolder;
            letter-spacing:-3em;
            animation: fadeInText 2s ease-in-out forwards;
            transition: color 0.3s ease;
        }

        .char {
            display: inline-block;
            color: gold;
            font-size: inherit;
            font-family: "楷体";
            font-weight: bolder;
            letter-spacing: 60px;
            transition: font-size 0.3s ease, transform 0.3s ease;
        }
    
        .char:hover {
            font-size: 6em;
            transform: scale(1.2);
            cursor: pointer;
        }


        .header {
            text-align: center;
            margin-bottom: 20px;
        }

        .header h1 .char {
            display: inline-block;
            color: rgb(63, 210, 236);
            font-size: inherit;
            font-family: "楷体";
            font-weight: bolder;
            letter-spacing: 60px;
            transition: font-size 0.3s ease;
        }

        .character-list {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
            width: 80%;
            justify-content: center;
        }

        .character {
            width: 200px;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
        }

        .character:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .character h3 {
            margin-top: 0;
            color: #333;
        }

        .character p {
            margin: 5px 0;
            color: #555;
        }

        .character .contact::before {
            content: "📧 ";
        }

        .character .bio {
            text-align: justify;
        }

        .character-1 {
            background-color: lightblue;
            border: 2px solid navy;
        }

        .character-1 h3 { color: navy; }
        .character-1 p { color: navy; }

        .character-2 {
            background-color: #5cf496;
            border: 2px solid rgb(105, 188, 218);
        }

        .character-2 h3 { color: rgb(236, 29, 29); }
        .character-2 p { color: darkred; }

        .character-3 {
            background-color: #14EE34;
            border: 2px solid #bfe26d;
        }

        .character-3 h3 { color: #F30920; }
        .character-3 p { color: #F30920; }

        .character-4 {
            background-color: #D8F080;
            border: 2px solid #866A55;
        }

        .character-4 h3 { color: #866A55; }
        .character-4 p { color: #866A55; }

        .character-image {
            max-width: 100%;
            display: block;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>
            <span class="char">《</span>
            <span class="char">熊</span>
            <span class="char">出</span>
            <span class="char">没</span>
            <span class="char">》</span>
            <span class="char">主</span>
            <span class="char">要</span>
            <span class="char">人</span>
            <span class="char">物</span>
            <span class="char">介</span>
            <span class="char">绍</span>
        </h1>
    </div>
    <div class="character-list">
        <div class="character character-1">
            <h3>光头强</h3>
            <p>职位：伐木工人</p>
            <p class="contact">联系方式：gtq@example.com</p>
            <p class="bio">光头强是伐木场的工人，经常与熊大熊二斗智斗勇。</p>
            <img class="character-image" src="光头强.png">
        </div>

        <div class="character character-2">
            <h3>熊大</h3>
            <p>职位：森林守护者</p>
            <p class="contact">联系方式：xd@example.com</p>
            <p class="bio">熊大是森林里的大哥，总是保护着弟弟熊二不受伤害。</p>
            <img class="character-image" src="熊大.png">
        </div>

        <div class="character character-3">
            <h3>熊二</h3>
            <p>职位：森林守护者</p>
            <p class="contact">联系方式：xionger@example.com</p>
            <p class="bio">熊二是熊大的弟弟，喜欢吃蜂蜜，性格憨厚可爱。</p>
            <img class="character-image" src="熊二.png">
        </div>

        <div class="character character-4">
            <h3>团子</h3>
            <p>职位：山神</p>
            <p class="contact">联系方式：tuanzi@example.com</p>
            <p class="bio">团子是森林中的山神，拥有神奇的力量，守护着深山。</p>
            <img class="character-image" src="团子.png">
        </div>
    </div>
</body>
</html>
