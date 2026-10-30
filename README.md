# Global Semiconductor Supply Chain: Sanctions, AI Investment and Sovereignty

![Dashboard](dashboard/dashboard.png)

## About this project
Exploratory analysis of the Global AI Sovereignty & Hardware Supply Chain dataset: six related CSV files covering 12 countries from 2015 to 2025. I cleaned and checked every file in Python, answered 12 questions on trade, sanctions, investment and economic indicators, and built a Power BI dashboard from the results.

## Dataset
Global AI Sovereignty & Hardware Supply Chain, from Kaggle: [https://www.kaggle.com/datasets/moaz1911/global-ai-sovereignty-and-hardware-supply-chain]
The dataset mixes real and synthetic data (flagged by an is_synthetic column), so the findings show patterns and are not verified real-world figures.

## Questions explored
1. Do sanctions affect a country's trade volume?
2. Which country imposes the most sanctions?
3. Which countries prefer which supplier?
4. Which countries spend the most on AI infrastructure, and how large is it relative to GDP?
5. Does the public or the private sector invest more?
6. Which company has the largest share of trade volume?
7. Which hardware type carries the most trade volume?
8. Which country has the highest AI sovereignty index?
9. How has dedollarization changed over time?
10. How do countries compare on currency strength?
11. Is AI investment related to inflation?
12. Does geopolitical sensitivity relate to trade value?

## Key findings
- Sanctions and trade: the link is very weak (correlation 0.16). China's trade volume more than doubled from 2015 to 2025 while sanctions on it rose, so this dataset shows no clear evidence that sanctions reduce trade.
- Countries that impose sanctions (Netherlands, US, South Korea, Germany, France, Japan: about 130 to 150 each) are almost never the ones targeted.
- No importing country relies heavily on one supplier (top supplier share 7.6% to 16.6%), and no company dominates: Samsung leads with 13.5% of units.
- AI accelerators carry the largest share of traded units (17.4%).
- The US spends the most on AI infrastructure (about USD 740 billion), but Taiwan and the UAE spend a larger share of their GDP.
- Private investment is 61% of the total, driven by the US, Taiwan and South Korea.
- The US has the highest AI sovereignty index in 2025 (95.5). China, India and the UAE show the largest rise in the dedollarization index.
- AI investment and inflation show a moderate negative correlation (-0.57) across 12 countries, but it is fragile and driven largely by Pakistan.

## Tools used
Python (Pandas, NumPy, Matplotlib, Seaborn), Jupyter Notebook, Power BI Desktop

## Limitations
- The data is partly synthetic, and the indices are the dataset's own measures.
- Results are associations, not causes.
- The supplier column mixes chip designers, memory makers and equipment makers.
- The energy grid file was cleaned and checked but not used in the final analysis.

## What I learned
Checking every file before merging catches problems that don't raise errors, such as impossible negative percentages in the energy file. Correlating columns from different tables only works after merging on keys, not by row position. The choice of measure (count or sum, dollars or ratio to GDP) can change the answer.

## Author
Yash Pawar, BSc Data Science student, MIT ACSC Alandi, Pune
GitHub: https://github.com/yashpawar-ds
LinkedIn: https://www.linkedin.com/in/yash-pawar-aaa6ba382/
Kaggle: https://www.kaggle.com/yashpawar7053
