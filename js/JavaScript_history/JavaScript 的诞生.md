# JavaScript 的诞生

## 诞生

- 1993 年，国家超级电脑应用中心（NCSA）发表了 NCSA Mosaic，这是最早流行的图形接口网页浏览器，它在万维网的普及上发挥了重要作用。1994 年，Mosaic 的主要开发人员随即创立了 Netscape 公司，并雇用了许多原来的 NCSA Mosaic 开发者用来开发 Netscape Navigator，该公司的目标是取代 NCSA Mosaic 成为世界第一的网页浏览器。在四个月内，已经占据了四分之三的浏览器市场，并成为 1990 年代互联网的主要浏览器。
- 1995 年，网景招募了布兰登·艾克，目标是把 Scheme 语言嵌入到 Netscape Navigator 浏览器当中。但更早之前，网景已经跟昇阳合作在 Netscape Navigator 中支持 Java，这时网景内部产生激烈的争论。后来网景决定发明一种与 Java 搭配使用的辅助脚本语言并且语法上有些类似，这个决策导致排除了采用现有的语言，例如 Perl、Python、Tcl 或 Scheme。为了在其他竞争提案中捍卫 JavaScript 这个想法，公司需要有一个可以运作的原型。艾克在 1995 年 5 月仅花了十天时间就把原型设计出来了。
- 最初命名为 Mocha，1995 年 9 月在 Netscape Navigator 2.0 的 Beta 版中改名为 LiveScript，同年 12 月，Netscape Navigator 2.0 Beta 3 中部署时被重命名为 JavaScript[1][16]，当时网景公司与昇阳电脑公司组成的开发联盟为了让这门语言搭上 Java 这个编程语言“热词”，因此将其临时改名为 JavaScript，日后这成为大众对这门语言有诸多误解的原因之一。
- 微软公司于 1995 年首次推出 Internet Explorer，从而引发了与 Netscape 的浏览器大战。微软对 Netscape Navigator 解释器进行了逆向工程，创建了 JScript，以与处于市场领导地位的网景产品同台竞争。JScript 也是一种 JavaScript 实现，这两个 JavaScript 语言版本在浏览器端共存意味着语言标准化的缺失，发展初期，JavaScript 的标准并未确定，同期有网景的 JavaScript，微软的 JScript 双峰并峙。除此之外，微软也在网页技术上加入了不少专属对象，使不少网页使用非微软平台及浏览器无法正常显示，导致在浏览器大战期间网页设计者通常会把“用 Netscape 可达到最佳效果”或“用 IE 可达到最佳效果”的标志放在主页。
- 1996 年 11 月，网景正式向 ECMA（欧洲计算机制造商协会）提交语言标准。1997 年 6 月，ECMA 以 JavaScript 语言为基础制定了 ECMAScript 标准规范 ECMA-262。JavaScript 成为了 ECMAScript 最著名的实现之一。除此之外，ActionScript 和 JScript 也都是 ECMAScript 规范的实现语言。尽管 JavaScript 作为给非程序人员的脚本语言，而非作为给程序人员的脚本语言来推广和宣传，但是 JavaScript 具有非常丰富的特性。

## JavaScript 的设计缺陷

这里有三个客观原因，导致 Javascript 的设计不够完善。

1. **设计阶段过于仓促**

- Javascript 的设计，其实只用了十天。而且，设计师是为了向公司交差，本人并不愿意这样设计。另一方面，这种语言的设计初衷，是为了解决一些简单的网页互动（比如，检查"用户名"是否填写），并没有考虑复杂应用的需要。设计者做梦也想不到，Javascript 将来可以写出像 Gmail 这种极其庞大复杂的网页。

2. **没有先例**

- Javascript 同时结合了函数式编程和面向对象编程的特点，这很可能是历史上的第一例。而且直到今天为止，Javascript 仍然是世界上唯一使用 Prototype 继承模型的主要语言。这使得它没有设计先例可以参考。

3. **过早的标准化**

- Javascript 的发展非常快，根本没有时间调整设计。  
  1995 年 5 月，设计方案定稿；10 月，解释器开发成功；12 月，向市场推出，立刻被广泛接受，全世界的用户大量使用。Javascript 缺乏一个从小到大、慢慢积累用户的过程，而是连续的爆炸式扩散增长。大量的既成网页和业余网页设计者的参与，使得调整语言规格困难重重。  
  更糟的是，Javascript 的规格还没来及调整，就固化了
  1996 年 8 月，微软公司强势介入，宣布推出自己的脚本语言 Jscript；11 月，为了压制微软，网景公司决定申请 Javascript 的国际标准；1997 年 6 月，第一个国际标准 ECMA-262 正式颁布。
  也就是说，Javascript 推出一年半之后，国际标准就问世了。设计缺陷还没有充分暴露就成了标准。相比之下，C 语言问世将近 20 年之后，国际标准才颁布。
