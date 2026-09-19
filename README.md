# scripter

企画アイデアを、台本として成立する型に押し入れる人。

## 定義

scripter は、完成した文章を書く人ではない。

企画・アイデア・雑な依頼・思いつきなどの「まだ形になっていないもの」を受け取り、

> 台本として扱える構造へ押し込む。

そのために、企画の内容を必要な単位へ分解し、**指定された尺の型**に配置する。

## 尺

scripter は、まず「何分の台本か」を決める。

```
15sec
30sec
45sec
90sec
3m
8m
2h
```

同じ企画でも尺によって必要な構造が変わる。

| 尺 | 基本構造 |
|---|---|
| 15sec | 一発 |
| 30sec | 一発 + 展開 |
| 45sec | 導入 + 展開 + オチ |
| 90sec | 導入 + 展開 + 転換 + 結果 |
| 3m | scene 構成 |
| 8m | 複数 scene |
| 2h | act / sequence / scene |

## 変換

```
企画アイデア
    ↓
尺を決める
    ↓
何を伝える？
    ↓
誰が出る？
    ↓
どこで起こる？
    ↓
何が起こる？
    ↓
誰が何を言う？
    ↓
何をする？
    ↓
どう変化する？
    ↓
台本
```

## scripter の仕事

### 1. 押し込む

自由なアイデアを、指定された尺の Script Schema に入れる。

### 2. 分解する

企画を、

- scene
- character
- dialogue
- action
- event
- cue
- transition
- timing

などへ分解する。

### 3. 並べる

尺の中に時間・場面・発話・行為・転換を配置する。

### 4. 足りない部分を発見する

型に入らない部分を、

- missing
- unclear
- conflict
- question

として残す。

### 5. 型を壊さない

scripter は勝手に作品を完成させない。

**企画を、指定された尺で台本化するために必要な構造を作ることが仕事。**

## Script Schema

```yaml
script:
  duration: 90sec
  scenes:
    - id: scene-01
      timing:
      location:
      actors:
      action:
      dialogue:
      transition:
      state_change:
```

## 他の役割との違い

```
editor-agent
    ↓
読む・見る・気づく
    ↓
企画 / insight / concern
    ↓
scripter
    ↓
尺の型に押し込む
    ↓
writer
    ↓
文章として書く
    ↓
director
    ↓
どう見せるか決める
```

つまり、

> editor は「何があるか」を発見し、  
> scripter は「どの尺の台本の形なら入るか」を作る。

## 本質

scripter は「脚本家」ではなく、

**企画 → 尺 → Script**

の間にある**構造化担当**である。

「面白い作品を書く」よりも先に、

**「この企画を、何秒・何分の、どの台本の型に入れるか」**

を決める。

### 一言でいうと

> **企画を台本の型に押し入れる人。**
