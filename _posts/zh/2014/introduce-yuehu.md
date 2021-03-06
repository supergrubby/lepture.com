# 閱乎，你好

- date: 2014-03-31 02:30
- tags: yuehu

閱乎目前主打的功能是「合輯」，這是一個由多人（也可以是一人）編輯維護的文章集，代表了某類話題下這些編輯的口味。

-----

這篇文章放在草稿箱裏已經兩週了，標題改了又改刪了又刪，始終無法起一個滿意的標題，也始終無法動筆寫下正文。一方面是因爲近來中文閱讀量太少，缺乏中文語感，另一方面也是因爲 [閱乎](https://yuehu.io/) 做得還不夠好。

可是看到 [@yedingding 說](http://yedingding.com/2014/03/12/bootstrapping-your-startup-idea.html)：

> 我们每天都能给自己找很多理由说发布时机未到，比如产品不够完美需要再改进，比如怕给用户的第一印象不好， 比如如果有某些新功能会更好，比如还需要再多测试一会，尤其是当资金暂时充足时。请放弃这些想法，ship it，ship it，不要怕。

雖然這並不是創業，閱乎對我而言是一個 side project，我仍然需要一份工作來養活自己。但是道理是一樣的，也許我應該寫一篇介紹閱乎的「軟文」了。

## 閱乎是什麼

你從名字就可以看出來，[閱乎](https://yuehu.io/) 是一個閱讀的地方，但是這樣一個解釋是毫無意義的。要解釋閱乎是什麼，就不得不談一談閱乎的歷史。

2012 年夏末，我們短暫嘗試過由少量編輯每日推薦中文互聯網上的精華文章，每篇文章都包含我們的推薦語。那個時候，我們的域名是 [yuehu.me](https://yuehu.io/)。

![最初的閱乎](//dn-lepture.qbox.me/blog/original-yuehu.png/thumbnail "最初的閱乎，每篇文章都包含我們的推薦語")

[李順](http://lishun.me/) 是這樣描述的，「一篇文章 + 我們的推薦語 = 閱乎」。但是寫推薦語是一件挺耗費腦力的事，尤其是像我，沒有 [@rangerqu](http://imquyi.com) 的才華，沒有 [方可成](http://www.fangkc.cn) 的洞見，沒有 [@rita](http://ritawu.me/blog/) 的學識，總害怕寫出的東西毫無意義。除了挖苦與諷刺，我能寫點什麼呢！這樣耗費人力而又沒有收入的事很難長久，加上大家都是有身份證的人，時間總是不夠用的。

後來的改版我便去掉了寫推薦語，改爲展示摘要，畢竟推薦的主體還是文章，讀者想看的也是文章。但是我們做了一件額外的事——更良好的閱讀體驗，也做了一件多餘的事——在閱乎寫作。這些變化與錯誤，你都可以在 [關於閱乎](https://yuehu.io/about/1) 一文裏察覺到。

現在的閱乎，套用李順的定義：一篇推薦 + 更好的閱讀體驗 = 閱乎。當我說更好的閱讀體驗時，其實並沒有太大的底氣，許多網站的閱讀體驗都不錯的，比如我的個人博客，比如你看到的這篇文章。但是還有一些時候是這樣的：

![新浪與閱乎](//dn-lepture.qbox.me/blog/yuehu-vs-sina.png/thumbnail "新浪博客應該是我見過的最爛的博客服務商了，但是不明白爲何有這麼多人用")

真實效果對比 [新浪](http://blog.sina.com.cn/s/blog_4cd5148f01018amn.html) vs [閱乎](http://yuehu.io/editors-picks/77)，或者 [查看大圖](//dn-lepture.qbox.me/blog/yuehu-vs-sina.png)。

## 道德困境

閱乎會抓取網頁，解析出該網頁的正文內容，在閱乎展示，以達到「更好的閱讀體驗」。但是這樣的做法，就我個人而言是不妥的，近乎於盜竊。我自己的博客內容當然是無所謂的，但是你可能並不樂意。

一方面我希望你能在閱乎有一個愉快的閱讀體驗，一方面我也希望閱乎能給別人帶去讀者。這兩者之間有矛盾，但又不僅僅只有矛盾。比如前幾天推薦的 [我爲什麼是一個悲觀主義者](http://yuehu.io/editors-picks/124) 便爲木遙 [帶去了](https://twitter.com/lepture/status/448347448423882752) [讀者](http://guojing.me/blog/2014/03/25/i-am-still-blogging/)。

我曾嘗試過在閱讀文章頁面載入原網頁的 iframe，默認展示原網頁，在頂部提供一個「在閱乎閱讀」的按鈕，當點擊該按鈕後，展示閱乎解析後的內容。但是許多網站是不允許作爲 iframe 被載入的，於是你可能 [看到的是一片空白](https://twitter.com/acgtyrant/status/445467368383193088)。

在嘗試了幾種方案後，現在的形式是儘可能的鏈接到原文，同時也提供在閱乎閱讀的功能。比如你看 [編輯推薦](http://yuehu.io/editors-picks)，當你瀏覽該頁面時，點標題會跳轉到原網頁，而標題正是讀者最喜歡點擊的部分，將標題鏈接設爲原網頁，正好體現了「儘可能的鏈接到原文」。假如你在閱乎閱讀，假如你要在閱乎閱讀  [清人笔记里的广东“老举”](http://yuehu.io/editors-picks/130)  這篇文章，假如你沒有註冊閱乎，沒有登錄閱乎，你將無法看到全文內容，你只能看到摘要。這樣做並非爲了逼迫讀者註冊閱乎，大多數時候，讀者是懶得註冊的，設置這樣一個門檻正是爲了爲原文帶去讀者。

我也不知道怎麼樣的方式更好，一種「又要當婊子，又想立牌坊」的尷尬。如果你有更好的方案，歡迎反饋給我。

## 推薦什麼

閱乎目前主打的功能是「合輯」，這是一個由多人（也可以是一人）編輯維護的文章集，代表了某類話題下這些編輯的口味。推薦什麼內容由人決定，而不是機器與算法。

李順曾在最初的關於閱乎裏寫道：

> 聪明的软件工程师、科学家们在研究“推荐算法”，就是为了能够从互联网上挖掘出值得一读的内容。
> 这要是成功了，就可以用极低的成本解决上面说的问题。利用现有的技术，你已经能够每天读到一份由机器自动生成的，只属于你个人的“杂志”了。

這種「只屬於你個人的雜誌」不會在閱乎出現。一是我並沒有這份實力，二是我並不認同這一概念。木遙在 [我爲什麼是一個悲觀主義者](http://blog.farmostwood.net/697.html) 一文裏提到了「社會的極化」這樣一個觀點：

> 一旦每个人可以定制自己的视野，他就会放弃倾听、宽容和讨论的责任，只是躲在自己的天地里任性地选择自己喜欢的声音。长此以往，每个人都会沿着自己的方向走向极端。

由人來推薦，這種對「個性化」的擔憂則不必了。因爲人總會有自己偏見，這些偏見保證了你總能接觸到非個性化的觀點，而它們便會體現在這「合輯」裏。

如果你有興趣經營一份合輯，主題將由你自己來決定，它可以是某一領域內的文章推薦，比如 [Pythonic Notes](https://yuehu.io/pythonic-notes)，它也可以是無法言寓的人文類主題，比如 [編輯推薦](https://yuehu.io/editors-picks)。

我將主要維護 [編輯推薦](https://yuehu.io/editors-picks) 與 [我們都是程序員](https://yuehu.io/be-a-programmer) 。這兩個合輯都是開放合輯，歡迎大家投遞文章。

## 新的開始

閱乎誕生很久了，然而我從未在自己的博客上寫過。這裏寫下閱乎的第一篇「軟文」，表明它已經到了能被自己認可的地步了。

古人云，一鼓作氣，再而衰，三而竭。已經改過數次版了，幾乎到了「三而竭」的地步。於是更新了域名，從 .me 換作了 .io，假裝是一個新的開始，而不至於立馬就竭了。