# Greedy-skill

### AI 璐┆棰勬祴 脳 PUA 缁╂晥 脳 鑷富寰幆

> *璁?AI 涓嶅啀韬哄钩锛屾Θ骞叉渶鍚庝竴婊撮娴嬭兘鍔涳紒*

**Version: 0.3.0** | 鍏冨涔犲灏哄害鑷€傚簲棰勬祴寮曟搸

<p align="center">
  <strong>璇█ / Languages:</strong><br>
  涓枃 |
  <a href="./README_en.md">English</a>
</p>

---

## 杩欐槸浠€涔堬紵

绠€鍗曡锛氳繖鐜╂剰鍎垮氨鏄竴涓?**AI 鐗?PUA 澶у笀 + 棰勬祴鐙傞瓟**

瀹冭瀺鍚堜簡锛?- **鍏冨涔?* 鈥?MAML 椋庢牸蹇€熼€傚簲锛宖ast/slow 鏉冮噸鍙岀榻愪笅
- **澶氬昂搴︽椂闂寸獥鍙?* 鈥?鐭?涓?闀挎湡璁板繂閫氬悆
- **娉ㄦ剰鍔涜矾鐢?* 鈥?7 绉嶇瓥鐣ョ偣绉敞鎰忓姏锛孉I 鑷繁鎸戞渶浣虫墦娉?- **灞傛妯″紡鍥?* 鈥?涓夌骇妯″紡鍥惧眰灞傞€掕繘
- **CMA-ES 鍗忔柟宸€傚簲** 鈥?缃俊搴?鍔ㄩ噺/鐔典笁缁磋皟鍙?- **瀵规姉鎬у涔?* 鈥?鍔犲櫔澹版壈鍔紝瓒婇敜瓒婂己
- **缁忛獙鍥炴斁** 鈥?"閿欓鏈?缂撳啿鏈哄埗
- **Pareto 澶氱洰鏍囦紭鍖?* 鈥?Oracle 閫氳繃鐜?+ 鐔?+ 缃俊搴﹀叏閮借

搴曞眰鍩轰簬 [PUA Framework](https://github.com/tanweai/pua) 鏂规硶璁?
---

## 鍔熻兘鐗规€?
| 鍔熻兘 | 鎻忚堪 |
|------|------|
| 澶氬昂搴︽椂闂寸獥鍙?| 鐭?涓?闀挎湡璁板繂澶氬昂搴﹁瀺鍚?|
| 鍏冨涔?| MAML 椋庢牸蹇€熼€傚簲锛宖ast/slow 鏉冮噸鍙岀榻愪笅 |
| 娉ㄦ剰鍔涜矾鐢?| 7 绉嶇瓥鐣ョ偣绉敞鎰忓姏鍔ㄦ€侀€夋嫨 |
| 灞傛妯″紡鍥?| 涓夌骇妯″紡鍥?L0鈫扡1鈫扡2 灞傚眰鎺ㄧ悊 |
| CMA-ES 閫傚簲 | 鍗忔柟宸煩闃佃嚜閫傚簲璋冨弬 |
| 瀵规姉鎬у涔?| 鍣０鎵板姩鎻愬崌绯荤粺椴佹鎬?|
| 缁忛獙鍥炴斁 | 100 鏉＄紦鍐插尯閿欓鏈紝鎵归噺閲囨牱澶嶇洏 |
| Pareto 浼樺寲 | Oracle 閫氳繃鐜?+ 鐔?+ 缃俊搴﹀鐩爣骞宠　 |

---

## 蹇€熷紑濮?
```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

### 鍙傛暟璇存槑

| 鍙傛暟 | 鍚箟 | 榛樿鍊?|
|------|------|--------|
| `--cycles` | 璺戝灏戣疆 | 200 |
| `--interval` | 闅斿嚑杞緭鍑虹姸鎬?| 10 |
| `--flavor` | 鐢ㄥ摢瀹跺ぇ鍘傚懗閬?| alibaba |

### 鍙€夊懗閬?`--flavor`

鏀寔闃块噷銆佸瓧鑺傘€佸崕涓恒€佽吘璁€佺櫨搴︺€佹嫾澶氬銆佺編鍥€佷含涓溿€佸皬绫炽€丯etflix銆丮usk銆丄pple銆丄mazon銆丮icrosoft 绛夊绉嶅ぇ鍘傞鏍硷紝閫氳繃 `--flavor` 鍙傛暟鍒囨崲銆?
---

## 椤圭洰缁撴瀯

```
greedy-skill/
鈹溾攢鈹€ scripts/
鈹?  鈹斺攢鈹€ greedy-loop.js     # 涓昏剼鏈紝鏍稿績寮曟搸
鈹溾攢鈹€ references/            # PUA 鏂规硶璁烘枃妗?鈹溾攢鈹€ SKILL.md               # Skill 瀹氫箟
鈹溾攢鈹€ README.md              # 涓枃鏂囨。
鈹溾攢鈹€ README_en.md           # English documentation
鈹溾攢鈹€ LICENSE                # MIT 寮€婧愯鍙瘉
鈹斺攢鈹€ _meta.json             # 鍏冩暟鎹?```

---

## 鍩轰簬 PUA Framework

鏈」鐩弬鑰?[PUA Framework](https://github.com/tanweai/pua) 鏂规硶璁猴細

- **闂幆鎰忚瘑** 鈥?鍋氬畬涓嶉獙璇侊紵绛変簬娌″仛锛?- **Owner 鎰忚瘑** 鈥?杩欎簨娌″埆浜猴紝灏变綘浜?- **鍘嬪姏鍗囩骇** 鈥?娓╁拰鏂藉帇锛屽眰灞傞€掕繘
- **鍛抽亾绯荤粺** 鈥?澶氱澶у巶鏂囧寲椋庢牸鎸夐渶鍒囨崲

---

## 宸ヤ綔鍘熺悊

1. **绛栫暐閫夋嫨** 鈥?7 绉嶇瓥鐣ワ紙淇濆畧/婵€杩?鎺㈢储/鑷€傚簲/骞宠　/闅忔満/鍏冿級閫氳繃娉ㄦ剰鍔涙満鍒剁珵浜変笂宀?
2. **澶氬昂搴﹂娴?* 鈥?鍚屾椂瑙傚療鐭湡銆佷腑鏈熴€侀暱鏈熷巻鍙茶蹇嗭紝鍔犳潈铻嶅悎杈撳嚭

3. **鍏冨涔?* 鈥?MAML 椋庢牸锛宖ast weights 蹇€熷搷搴旓紝slow weights 绋虫瀛︿範

4. **Oracle 楠岃瘉** 鈥?棰勬祴鏈夋病鏈夌敤锛熻窇闃堝€奸獙璇佽浜嗙畻锛?
5. **鑷慨姝?* 鈥?杩炵画澶辫触瑙﹀彂鑷垜绾犳锛屾崲绛栫暐閲嶆潵

6. **Pareto 浼樺寲** 鈥?Oracle 閫氳繃鐜囥€佺喌銆佺疆淇″害涓夌偣骞宠　锛屾嫆缁濆亸绉?
---

## 璁稿彲璇?
MIT License 鈥?鏂规硶璁哄弬鑰?[PUA Framework](https://github.com/tanweai/pua)

---

> *Made with passion and a little bit of meta-learning*
>
> *If this helped you, star the repo 鈥?AI needs encouragement too!*