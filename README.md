# CSM-MTBench

Data for our paper "Benchmarking Machine Translation on Chinese Social Media Texts". 

One can find data in corresponding folders. We split them based on language directions.

## Fun Posts
Fun Posts are longer, content-rich user posts that typically describe events, experiences, or personal observations, often containing slang and neologisms.

### Data Structure (zh->ja Example)

```jsonc
{
  "source": "我去，感觉完全变了个人",  // Chinese source sentence
  "slang": "我去",                  // slang or neologism in this sentence
  "slang_trans": "マジで",          // glod label translation for the slang or neologism
  "slang_candidates": [
    "まじか",
    "まじかよ",
    "うわっ",
    "やばっ",
    "うそでしょ",
    "え、まじ？",
    "なんてこった"
  ],                               // a list for other reasonable expression of the slang in the target language
  "translation": "マジで,まるで別人になったような感じがする。" // Human annotated gold label translation
}
```

## Social Snippets
Social Snippets capture short, highly emotional or reactive user comments, often exhibiting distinctive tones and stylistic features. 

### Data Structure (zh->ja Example)

```jsonc
{
  "source": "已关注，莫辜负",                    // Chinese source sentence
  "translation": "フォロー済み、裏切らないでね",   // Human annotated gold label translation
}
```

## Evaluation
Please refer to our paper on how to implement evaluation for now. (XCOMET, SSR, ES, GEMBA)

Evaluation codes will be available soon. (Currently under internal company review)
