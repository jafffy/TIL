# express-generator

문제
---
Learning Node 책을 보는데, 여기서 express framework 기반의 project hierarchy를 만들 때, 아래와 같이 하라고 나와 있었다.

~~~bash
npm install express
express site
~~~

하지만 내 terminal(OSX)은 연신 express를 찾을 수 없다고 외쳐댔고, 나는 대안을 찾아서 검색을 시작했다.

해결
---
답은 [express-generator](https://expressjs.com/en/starter/generator.html)였다.

위 튜토리얼에서 시키는대로,

~~~bash
npm install express-generator -g
~~~

를 수행한 후에

~~~bash
express site
~~~

라고 적용하니 원하는 결과가 나왔다.

트라비아(1)
---------
그건 그렇고, 나는 의도하지 않았는데 현재 하는 dashboard project에 angular.js, express.js, node.js를 쓰고 있었다!

내 요구사항 분석에 따르면 dashboard project는 scalability를 비롯한 성능 문제도 없고, reliability 문제도 없다. 그냥 잘 떠있다가, 10명 미만의 사용자들이 접속해서 잘 돌아가면 되는 웹 서비스이기 때문이다.

나도 모르게 MEAN을 완성해 가는 것을 보며, 역시 시간과 노력을 아끼는 방법으로써의 MEAN은 훌륭한 대안이구나, 싶었다.

트라비아(2)
---------
나는 npm eco system은 물론이고 웹 자체에 대해서 하나도 모르는 사람이다. 그래서 아래와 같은 것도 몰랐다.

~~~bash
npm start
~~~

그냥 express로 generate한 프로젝트에서 위 커맨드를 치니 localhost에서 접근할 수 있는 deploy가 됐다. 신기하다.
