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
            },...
          ]
        },...
      ]
    }
  ]
}
```

### Data Format - CMRC
```
{ 
  "version": "v1.0", 
  "data": [
    {
      "paragraphs": [
        {
          "id": "DEV_0",
          "title": "战国无双3", 
          "title_label": 0, 
          "context": "《战国无双3》（）是由光荣和ω-force开发的战国无双系列的正统第三续作。本作以三大故事为主轴，分别是以武田信玄等人为主的《关东三国志》，织田信长等人为主的《战国三杰》，石田三成等人为主的《关原的年轻武者》，丰富游戏内的剧情。此部份专门介绍角色，欲知武器情报、奥义字或擅长攻击类型等，请至战国无双系列1.由于乡里大辅先生因故去世，不得不寻找其他声优接手。从猛将传 and Z开始。2.战国无双 编年史的原创男女主角亦有专属声优。此模式是任天堂游戏谜之村雨城改编的新增模式。本作中共有20张战场地图（不含村雨城），后来发行的猛将传再新增3张战场地图。但游戏内战役数量繁多，部分地图会有兼用的状况，战役虚实则是以光荣发行的2本「战国无双3 人物真书」内容为主，以下是相关介绍。（注：前方加☆者为猛将传新增关卡及地图。）合并本篇和猛将传的内容，村雨城模式剔除，战国史模式可直接游玩。主打两大模式「战史演武」&「争霸演武」。系列作品外传作品",         
          "qas": [
            {
              "question": "《战国无双3》是由哪两个公司合作开发的？", 
              "id": "DEV_0_QUERY_0", 
              "answers": [
                {
                  "text": "光荣和ω-force", 
                  "answer_start": 11
                },...    ], 
            }, ...],
       }, ...]
}
        
```
