<template>
  <h1 class="NAVITIME">{{company.name}}</h1>
  <h1 class="years">{{company.sinceyear}}</h1>
  
  <img class="src" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTXzYmT8sRYQERcaifzkPbVFDraSU3Gh2h1aA&s" alt="熱中症の少年イラスト" />
   <h3 class="charactar">会社の特徴</h3>
  <p class="honbun">株式会社ナビタイムジャパンは、2000年3月1日に設立された東京都港区に本社を置く企業です。
    代表取締役は大西啓介氏（工学博士）が務め、2025年4月現在の従業員数は430名、資本金は9,000万円です。
    同社は経路探索およびナビゲーションを基軸としたサービスを開発・提供しており、「NAVITIME」アプリの運営・開発だけでなく、
    経路探索エンジンのライセンス事業、動態管理ソリューション、MaaS事業など多岐にわたる分野で事業を展開しています。

1996年に経路探索エンジンのライセンスビジネスを開始し、1998年には世界初のトータルナビゲーションを完成させました。
その後、2001年に「NAVITIME」サービスの提供を開始し、法人向けサービスや海外向けサービス、インバウンド事業へと拡大しています。
経営理念として「経路探索エンジンの技術で世界の産業に奉仕する」ことを掲げ、独自の経路探索アルゴリズムをコア技術として、
社会の様々な移動課題の解決に貢献しています。安定した経営基盤も特徴で、過去10年間赤字決算がない実績を持っています。</p>

  <h3 class ="useTech">使用技術</h3>
  <ul class="Techs">
    <li>JavaScript</li>
    <li>Python</li>
    <li>react</li>
  </ul>

  <div class="top"></div>
  <div class="bg_pattern Paper_v2"></div>
  <input type="text" placeholder="スキルを入力"/>
  <button type="button">追加</button>
  <ul>
    <!--
    <li class="tenki">明日の天気は{{text1}}です。</li>
    <li class="tenki2">明日の天気は{{array[0]}}です。</li>
    <li>{{a}}</li>
    -->
  </ul>
  
</template>

<script setup>
  const weather = '晴れ';
  let text1 ="くもり";
  text1 ="雨";
  const company={
    name:"NAVITIME",
    sinceyear:"3DAYS インターン体験記"
  };
  console.log(company.name);
  const array =[114514,2,3]
  console.log(array[0])
  const a="高校時代は山岳部でした";

</script>

<style>
.NAVITIME {
  
  display:flex;
  color: #42b983;
  margin-top: 20px;
  margin-left: 300px;
  margin-right:20px ;
  margin-bottom: 20px;

}
.years{
  display:flex;
  margin-top:20px;
  margin-left:200px;
}
.Python {
  color: #42b983;
}

.red {
  color: black;
}

.Techs{
  justify-content: center;
  display: flex;
  list-style: none;
  padding: 10px;
}

li{
  margin-right:20px;
}
.tenki2{
  color: red;
}
.charactar{
  display:flex;
  align-items: center;
  margin-top: 50px;
  margin-left: 330px;
}
.src{
  max-width: 30%; /* 親要素の幅を超えない */
  height: auto; /* 縦横比を維持 */
  display: block; /* ブロック要素化してmargin autoを効かせる */
  margin: 20px auto; /* ★変更: 中央寄せと上下余白 */
  border: 1px solid #ddd; /* 軽く枠線 */
  border-radius: 8px; /* 角を丸く */
  box-shadow: 0 2px 5px rgba(0,0,0,0.1); /* 影 */
}
.useTech{
  display: flex;
  padding: 10px;
  margin-top: 50px;
  margin-left: 330px;
}
.bg_pattern {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: #fff;
  z-index: -1;
}
.Paper_v2 {
  background-image:
    repeating-linear-gradient(to bottom,
      transparent 25px,
      rgba(0, 0, 0, 0.04) 26px,  rgba(0, 0, 0, 0.04) 26px,
      transparent 27px,  transparent 51px, 
      rgba(0, 0, 0, 0.04) 52px,  rgba(0, 0, 0, 0.04) 52px,
      transparent 53px,  transparent 77px, 
      rgba(0, 0, 0, 0.04) 78px,  rgba(0, 0, 0, 0.04) 78px,
      transparent 79px,  transparent 103px, 
      rgba(0, 0, 0, 0.04) 104px,  rgba(0, 0, 0, 0.04) 104px,
      transparent 105px,  transparent 129px, 
      rgba(0, 0, 0, 0.04) 130px,  rgba(0, 0, 0, 0.04) 130px),
  
    repeating-linear-gradient(to right,
      transparent 25px,
      rgba(0, 0, 0, 0.04) 26px,  rgba(0, 0, 0, 0.04) 26px,
      transparent 27px,  transparent 51px, 
      rgba(0, 0, 0, 0.04) 52px,  rgba(0, 0, 0, 0.04) 52px,
      transparent 53px,  transparent 77px, 
      rgba(0, 0, 0, 0.04) 78px,  rgba(0, 0, 0, 0.04) 78px,
      transparent 79px,  transparent 103px, 
      rgba(0, 0, 0, 0.04) 104px,  rgba(0, 0, 0, 0.04) 104px,
      transparent 105px,  transparent 129px, 
      rgba(0, 0, 0, 0.04) 130px,  rgba(0, 0, 0, 0.04) 130px);
}




</style>
