<img src="./images/image0001.jpg" alt="Image of the Store Interior" width="400px">

## → Foreword  

🔺Accent Sisters bookstore moved to Union Square in spring. They needed to overhaul their book inventory, which mostly included Chinese books and niche titles from independent or small presses. I had no prior experience with Shopify or inventory management. Shopify was their only inventory record, but it was incomplete and inaccurate. Initially, manual entry was proposed, but after some failed attempts, I decided to automate the process using ISBN scanning, web scraping, API requests, data cleaning in Python, and Zotero.

🔺Written in a fun, storybook style and in two languages, this tutorial documents my journey in creating and troubleshooting this workflow. Included are Python tutorials for web scraping (with BeautifulSoup and Selenium), data cleaning strategies, and practical guidance for anyone looking to retrieve bulk information about Chinese-language books: which sources work, which ones don’t, and the data cleaning challenges that inevitably follow.

---

## → 楔子  

🔺Accent Sisters书店在春季搬到了联合广场的新址，需要对店里的书籍库存进行一次全面盘点和整理。这些书籍大部分为中文书以及一些独立出版或小众出版社的图书。我之前没有用过Shopify，也没有库存管理经验。店里唯一的库存记录就是Shopify，但这个记录并不完整，且数据不准确。最初店方提出的是手动录入书籍信息，但在尝试过并失败后，我决定通过ISBN扫描、网络爬虫、API请求、Python数据清理和少量Zotero辅助来实现自动化的解决方案。

🔺本教程以轻松、有趣的双语故事形式撰写，记录了我在设计与调试整个工作流程中的过程，包括利用Python进行网络爬取（BeautifulSoup和Selenium）、数据清理方法，以及提供给其他同样需要批量获取中文图书信息的人一些实用建议：哪些信息源可用、哪些信息源不可用，以及后续可能遇到的数据清理难题。

---

## → File Structure  
```text
├── Data/ # Sample datasets used in the tutorial
│ ├── dangdangResults.csv
│ ├── isbndbResults.csv
│ ├── scannedResults.csv
│ └── zoteroExport.csv
│
├── Story/ # Tutorial and story chapters with code examples
│ ├── Chapter1.md
│ ├── Chapter2.ipynb
│ ├── Chapter3.ipynb
│ ├── Chapter4.ipynb
│ ├── Chapter5.ipynb
│ ├── Chapter6.ipynb
│ └── Forward.md
│
├── images/ # Images used in the story/tutorial
│ └── image0001.jpg
```
---

## → Notes  

- The `Data/` folder contains all CSV files generated or used in the scraping and metadata merging steps.
- The `Story/` folder documents the entire pipeline and its development as a bilingual narrative tutorial.
- The `images/` folder contains all referenced screenshots, interface images, and annotated visuals.

This README provides context for navigating and reproducing the pipeline described in the story chapters.
