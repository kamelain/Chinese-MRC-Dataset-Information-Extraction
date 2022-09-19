# Chinese-MRC-Dataset-Information-Extraction
DRCD-Information-Extraction, CMRC-Information-Extraction

### Dataset
Clustering title or keywords in [DRCD](https://github.com/DRCKnowledgeTeam/DRCD) , [CMRC](https://github.com/ymcui/cmrc2018) into groups (pseudo-classes).

> "title_label": 1
> -> Passage group #1.


### Data Format - DRCD
```
{
"version": "1.3",
"data": [
  {
    "title": "基督新教",
    "id": "2128",
    "title_label": "1",
    "paragraphs": [
      {
        "context": "基督新教與天主教均繼承普世教會歷史上許多傳統教義，如三位一體、聖經作為上帝的啟示、原罪、認罪、最後審判等等，但有別於天主教和東正教，新教在行政上沒有單一組織架構或領導，而且在教義上強調因信稱義、信徒皆祭司， 以聖經作為最高權威，亦因此否定以教宗為首的聖統制、拒絕天主教教條中關於聖傳與聖經具同等地位的教導。新教各宗派間教義不盡相同，但一致認同五個唯獨：唯獨恩典：人的靈魂得拯救唯獨是神的恩典，是上帝送給人的禮物。唯獨信心：人唯獨藉信心接受神的赦罪、拯救。唯獨基督：作為人類的代罪羔羊，耶穌基督是人與上帝之間唯一的調解者。唯獨聖經：唯有聖經是信仰的終極權威。唯獨上帝的榮耀：唯獨上帝配得讚美、榮耀",
        "id": "2128-2",
        "qas": [
          {
            "id": "2128-2-1",
            "question": "新教在教義上強調信徒皆祭司以及什麼樣的理念?",
            "answers": [
              {
                "id": "1",
                "text": "因信稱義",
                "answer_start": 92
              }
            ]
          },
          {
            "id": "2128-2-2",
            "question": "哪本經典為新教的最高權威?",
            "answers": [
              {
                "id": "1",
                "text": "聖經",
                "answer_start": 105
              }
            ]
          },
          {
            "id": "2128-2-3",
            "question": "新教認同幾個唯獨?",
            "answers": [
              {
                "id": "1",
                "text": "五個",
                "answer_start": 171
              }
            ]
          },
          {
            "id": "2128-2-4",
            "question": "文中提及，人唯獨藉信心接受神的赦罪、拯救，此為哪一種唯獨?",
            "answers": [
              {
                "id": "1",
                "text": "唯獨信心",
                "answer_start": 206
              }
            ]
          }
        ]
      },...
    ]
  }
]
}
```
