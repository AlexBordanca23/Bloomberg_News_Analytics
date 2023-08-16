
# Analyzing COVID-19's Impact on Stock Prices #

***This Project was initially completed in the Fall Semester of 2020 as part of the Risk and Fluctuations in Financial Markets course at NYU College of Arts and Sciences.***

This research project investigates the significant impact of COVID-19-related news on stock prices during the exceptional year of 2020. The analysis focuses on coding daily market reports into fundamental, technical, and Knightian Uncertainty factors. The research employs the viewpoints of Rational Expectations Hypothesis, Behavioral Finance, and Knightian Uncertainty to explore the relationship between news and market sentiment.

## Key Achievements: ##

Data Categorization: The project effectively categorizes daily market reports, demonstrating a meticulous approach to capturing the diverse factors influencing stock prices.

Regression Analysis: Through regression models, the study establishes significant relationships between factors and market volatility. The analysis notably underscores the strong link between COVID-19 news and heightened market volatility.

Comparative Frameworks: The project provides a comprehensive assessment of three financial frameworks - Rational Expectations Hypothesis, Behavioral Finance, and Knightian Uncertainty. The evaluation offers insights into their applicability within the context of the data.

Insightful Conclusion: The research concludes that Knightian Uncertainty emerges as the most suitable framework for explaining the exceptional market behavior in 2020. This conclusion highlights the project's ability to synthesize complex concepts and apply them to real-world financial scenarios.

By delving into the intricate relationship between unforeseeable events, psychological factors, and market dynamics, this project demonstrates a deep understanding of finance and its practical implications during unprecedented times.


Alexandru Bordanca

ab7953

12/18/2020

**Final Paper on the Impact of Covid Related News on Stock Prices**

**Introduction**

2020 has been an almost unprecedented year from both social, economic and political perspectives. When taking into account the significant momentum the economy had displayed in the years since Trump’s election, the grinding halt that the global economy came to in light of the escalation of the COVID-19 pandemic was made that much more monumental. The fact that this was an election year, and each party and their respective candidates presented radically different approaches to mitigating the spread and economic effects of the virus made the personal and financial consequences of such an outbreak more disastrous. As of March, the UN has predicted a loss measured in the global economy at $1 trillion.[^1] This was further exaggerated by collapsing oil prices that saw gas at its cheapest point in over 5 years. Knightian Uncertainty is defined as true uncertainty where in fundamental change occurs in an unforeseeable manner and magnitude. If ever there was a year in which Knightian Uncertainty could be so liberally used to characterize events, it was 2020. Given that it has been such an eventful year, this paper shall focus more narrowly on the impact of the COVID pandemic on the economy.

Based upon research methodology outlined by Professor Nicholas Mangee, this paper seeks to determine the precise relationship between fundamental, technical and Knightian Uncertainty factors, in particular unforeseeable news related to the COVID pandemic and stock prices. The news is captured from the daily market wraps provided by Bloomberg. The research methodology is based on a coding of the aforementioned market wraps into subcategories of the categories of fundamental, technical, and Knightian Uncertainty (with particular emphasis on COVID) factors. Stock data is captured from the prices of the Big Three: The Dow Jones, The S&P 500, and the NASDAQ. In interpreting this data, we will employ three financial schools of thought: Rational Expectations Hypothesis, Behavioral Finance, and Knightian Uncertainty. We shall attempt to explain the data from the views and constraints by each school, ultimately comparing and contrasting how well they explain the data. 

It is however important for us to determine some important points in time as pertains to the data. While our data will mostly focus on the trading days between September 21, 2020 and December 11, 2020, we will examine certain breakpoints, or moments of high volatility in market swings, that lie outside of that range in determining causality between news and market movements. In terms of technical analysis, what we here mean by breakpoints can better be described as sharp, volatile reversals in asset price direction. In doing so we will examine the year to date (YTD) graphs of the Big Three and capture visually where such breakpoints occur within this year. 




![ScreenShot](https://raw.github.com/AlexBordanca23/Bloomberg_News_Analytics/main/figs/fig1.png)

*Figure 1— Normalized Price of Big Three Over Time*

Upon examining the overlayed graphs we see that though their price differs, and scaling might be an issue, they have the same general shape throughout the year 2020.  One important note I must make in analyzing this data is that due to the widely differing nominal prices between the three, in order to accurately overlay each of them in a plot, I had to normalize the price by dividing each daily price by the mean value of the index in question, over the year-to-date period up to December  11, 2020. We thus can establish several breakpoints: February 19, March 10, March 23, September 2, and November 9. Upon a review of the data we will include these dates, and search for a reason as they were so volatile in those days, ending in a short-term trend reversal and whether or not it was related to COVID. At first glance these breakpoints seem intuitive and we can connect the majority of them to some major KU event, and of that majority most seem initially related to COVID, with the other being related to an election result. The case can be made, however, that due to the vastly differing views on the pandemic by each respective candidate, that the election result in and of itself is inherently linked to the pandemic. In any case, we will pay special attention to these particular market wraps, if available, in our thorough analysis of the data. 

**Presentation of Data**



Within this section is a presentation of the data collected over the aforementioned time period of mid-September to mid-December. The data is far from perfect and the coding of the data itself within the categories outlined by Professors Mangee and Frydman is certainly subjective. The important aspects in considering the validity of this data are: a) the sample considered is larger than thirty so we can assume that the Law of Large Numbers and the normality of the distribution under the null is approximately normal; b) the coding, though subjective, is consistent as pertains to my interpretations of the Bloomberg Market Wraps, so extrapolations can be made. 

We first begin with a frequency table that captures the relative frequency of instances where certain categories are said to have directly influenced the movement of the stock market as captured by the Big Three indices. What is depicted below is the breakdown of instances of Fundamental, Psychological and Technical factors that moved the market, as well as relevant KU and more specifically COVID factors related to movements in the market. Within the first three categories, their respective top categories and their frequencies are also included in the table.




|Factors that Moved the Market|% Trading Days|
| - | - |
|Fundamentals|88\.9|
|`    `Government/Fiscal|59\.3|
|`    `Financial Institutions|37\.1|
|`    `Benchmark Valuation|33\.3|
|Psychological|40\.7|
|`    `Psychology with fundamentals|37\.1|
|`    `Pure Psychology|7\.4|
|Technical|33\.3|
|`   `Momentum|25\.9|
|`   `Non-Momentum|7\.4|

*Table 1 - Frequency of Factors that Moved the Market*

We can see from this table that there are strong fundamental factors driving the market, thus giving merit to the Rational Expectations Hypothesis school of thought, in an incidence comparable to what Mangee and Frydman observed over a much larger time period. Note that the sub percentages are not based on what part of their respective categories they comprised but rather what percentage they occurred on out of total days in the sample. This is with the exception of technical factors where the two subcategories are mutually exclusive. Differences between these results and the ones presented in Professor Mangee’s work can be attributed to difference in coding, sample size, and fundamental differences within the samples themselves. I contend that the period in which my data falls, is completely unique, due to both the magnitude and strangeness of the events of the year 2020. Let us further examine the data to see what truly moved the market over the time period in question.

Almost immediately we can observe that the biggest movers were government and fiscal news and psychology with fundamentals, most of that attribute being captured by psychology with government and fiscal news. There is also another key mover that is apparent, COVID — which I have treated as a KU factor — had a frequency of being mentioned of 66.7%.[^2] Further we must consider that due to the nature of pandemics to instill fear and panic, there is certainly a great deal of psychological factors included in the COVID factor, as well as in the technical factors such as momentum-based swings in the prices of the indices. Before we move further in the analysis, it is important to present, at minimum, an abridged version formalized dictionaries, filtered for relevance, used to capture the two largest movers, which are presented below:[^3]

- Government and Fiscal: Trump, Biden, Presidential Debate, White House, Senate, Stimulus, Legislation
- COVID: coronavirus, lockdown, pandemic, vaccine, clinical trials, hospitalizations, infections

These dictionaries, though shortened to better fit the final context of this paper, present the keywords in defining the volatile market climate that characterized the time period of mid-September to mid-December, and of the year 2020 as a whole.

Imagine we are interested in capturing the exact effect of these big movers, mainly the government and fiscal factors and the pandemic factors and the movements in financial markets. One way to capture, at least on a fundamental level, is via a frequency graph of these two main movers over time. We can then correlate the large spikes in those factors with major moves in the market or volatility in the market. As a proxy for volatility, to keep things simple, we can use the day range. Where we see large spikes, we look for the date, find the day range, and see what we can pinpoint in the news as the precise event falling under one category or another. Intuitively speaking, we can expect to more easily pinpoint the event in government or fiscal terms as there is less noise and the exact events are more precise, whereas with COVID the event may be something as general as more cases/hospitalizations or increased lockdowns. Keeping in mind the notion of the breakpoints outlined in the introduction and their implications on the news, below we shall present the frequency graphs and go through the process outlined above.


![ScreenShot](https://raw.github.com/AlexBordanca23/Bloomberg_News_Analytics/main/figs/fig2.png)
*Figure 2 - Daily Mentions of Each Mover*

This graph, though disorienting at first, captures the precise effects we are looking for. Therefore, we can determine that there are 3 major spikes at around October 7 and November 9. We will examine the index price data to determine the daily range for the Dow Jones Index, for the sake convenience. For October 7 and November 9, we observe a daily range of $626.45 and $803.17, respectively. In comparison to the average of $472.31, these are certainly significant daily ranges. The importance of the 9<sup>th</sup> of November is apparent, as an election result was finally made official in combination with a continued increase in COVID cases. This combination result in the largest intra-day range of the Dow Jones Industrial Average Index in the year 2020 to date. Meanwhile the 7<sup>th</sup> of October featured a continuation of the back-and-forth talks on a second round of stimulus. The latter is a characteristic that has been repeated almost continuously throughout the time period in which our sample falls. With that in mind, it is important to consider the extreme psychological ties to the market that these stimulus talks (as fundamental factors) have on repeatedly shifting the sentiment from optimistic to pessimistic and back to optimism in what has been a seemingly interminable negotiation process. In short, on the latter, point it is clear that, as a fundamental factor, a second round of stimulus would have a monumental impact on the economy and markets as a whole, however the psychological sentiment associated with these stimulus talks has certainly been a key element integral to explaining the volatility observed in the market this year. Therefore, at face value we can almost certainly conclude a very strong relationship between movement in the market and these election/stimulus and COVID factors.

`	`These results, though promising, are vague at best. In trying to find a more formal and precise relationship between these movers and volatility in the market, I also ran regression models on what are, as seen by the above frequency table, the largest movers of the stock market. These regressions were run as simple linear models in the R statistical programming language, and the stargazer outputs are emulated into the tables below. The results show the powerful relationship between the fundamental and KU COVID factors that drove the market over the period in question. The variables used in the regression are defined as follows: Day Range is the difference between the daily High and Low, acting as a proxy for volatility; Government or Fiscal captures the daily mentions of political and fiscal factors such as election news and stimulus talks; and COVID measures the daily mentions of news related to the pandemic in the market wraps.

We first have the regression of Daily Range on both Government/Fiscal factors and COVID factors:


||**Day Range**|
| - | - |
|**GOV**|20\.957|
|**COVID**|65\.125\*|
|**Constant**|316\.178\*\*\*|
|**R-2**|0\.280|
|**Adj. R-2**|0\.220|
|**F-Statistic**|4\.666\*\*|
|The COVID Factor is significant at the 10% level while the model itself is significant at 5%|

*Table 2 - Regression of Daily Range on Both GOV and COVID*

This table certainly shows a lot of promise and immediately points out the significance of the COVID factor and the model is already significant at an acceptable level. There is however one issue associated with this model as it stands. One of the main keywords that comprise the GOV factor is stimulus and stimulus negotiations. Obviously, this is a term that is heavily related to the pandemic, thereby correlating our GOV factor to our COVID factor. Fundamental econometrics suggests that correlation or collinearity between independent variables may skew our model in one way or another, damaging its credibility. Therefore, in order to better capture the precise nature of the relationship between the volatility in the market and these factors, we must analyze the effect of each factor on daily range separately via regression of the range on only GOV and only COVID. Below we shall analyze the relationship between the GOV factor and the Daily Range.


||**Day Range**|
| - | - |
|**GOV**|53\.155\*\*|
|**Constant**|362\.358\*\*\*|
|**R-2**|0\.164|
|**Adj. R-2**|0\.130|
|**F-Statistic**|4\.887\*\*|
|The Government or Fiscal Factor is significant at the 10% level while the model itself is significant at 5%|

*Table 3 - Regression of Daily Range on GOV*

Immediately we see that the significance of both the GOV factor and our model has improved so we can consider this to be a step in the right direction. However, given the nature of this past year and how heavily impacted it has been by the pandemic, it seems illogical to leave out what appears to be such an important factor. To conclude our regression analysis, let us regress daily range on strictly COVID factors.




||**Day Range**|
| - | - |
|**COVID**|79\.538\*\*\*|
|**Constant**|319\.277\*\*\*|
|**R-2**|0\.263|
|**Adj. R-2**|0\.234|
|**F-Statistic**|8\.931\*\*|
|The COVID Factor is significant at the 1% level while the model itself is significant at 1%|

*Table 4 - Regression of Daily Range on COVID*

We immediately see the most significance in any of our three models, with both the explanatory variable and the model itself being significant at the 1% level. It has an R-2 constant comparable to the first model, but much greater significance. But why is it that excluding the GOV factors automatically gives the model a higher level of significance. I postulate that it is due to the correlation between the stimulus talks and the pandemics alluded to above. The pandemic has even further reaching causality in the set of GOV factors and keywords; even the election itself, given the vast difference in how the candidates intend to approach the pandemic, can be characterized in terms of COVID. That being said, we cannot completely rule out the relationship between strictly GOV and daily range as the differences in the candidates’ macroeconomic policies is characterized by ideology rather than by response to the pandemic. However, as the Bloomberg wraps indicate, market participants anticipate that should Biden win, a Republican senate and attempts to win midterm elections will keep his aggressive tax plan at bay, thereby allowing the markets to prosper. With that in mind — though it cannot be completely ruled out —in comparison to the COVID factor within the context of this sample, the significance of the GOV factor is at best marginal. 

**Comparison of the Analysis Across the Three Schools**

Up to this point in the paper we have analyzed the data from a strictly quantitative perspective. We shall now try to make light of the data within the context of each of the three schools of thought: Rational Expectation Hypothesis, Behavioral Finance, and Knightian Uncertainty. Since each school has a fundamentally different intuition as to which factors and precisely how those factors drive the stock market, the data can be interposition to create a very nice comparison between the three schools. In comparing them, we will analyze the main tenets of each school’s approach to explain how the market works and what drives prices, and how the data can be contextualized within this school and whether or not the data supports or rejects the notions brought on by the school.

We begin with the Rational Expectations Hypothesis. This school of thought hinges on the idea that strictly fundamental factors are the sole drivers of market movements. The present value construct found in most REH models characterizes the present value of an asset, stay a stock as the sum of the discounted future income streams, i.e. dividends, and the expected future value plus some error term. More sophisticated REH models can include macroeconomic data and political climate as factors affecting either of those variables, thus allowing us to use our entire fundamentals category from the data analysis in discussing the validity of REH in terms of the data. More importantly, REH models view psychology as irrationality. In order to move further, we must clearly define what is meant in this context as rationality to see what is or is not a departure from rationality. Muth made a groundbreaking leap in considering rationality thusly, albeit simply put: actions consistent with understanding of the processes driving the economy. Therefore, when constructing an REH model an economist must take into account the behaviors of market participants in their forecasts in a way consistent with their ends (profit). Based on this thought process the data certainly seems to give some degree of validity to the REH school of thought as fundamentals are mentioned frequently as driving the stock market. 

However, REH models do have one glaring issue: they assume away unforeseeable change. Going back to this year, who could have foretold of the pandemic let alone the magnitude of it? Assuming away such unforeseeable change that, as evidenced by the data, has been a significant factor in moving the stock market verges on irrationality. Going back to the regression analysis, let me highlight that the COVID factor was more statistically significant than the GOV factor. The other issue with REH models, particularly in the context of this data set is Shiller’s excess volatility puzzle. His analysis could not explain the excess volatility in actual prices versus fundamental price (*contra* REH) over a larger time frame, let alone over a year as volatile as 2020. Therefore, we must conclude that regardless of what the precise process that underpins the changes in dividends is, the fundamental value moves to slowly to capture the actual market. But what is the source of the volatility that is so prominent in our data set? As our regression models point out the pandemic has been a major driver of the volatility in the market. Clearly the nature of term pandemic implies a certain level of panic so we must turn to psychology to perhaps explain this, thus bringing us to the Behavioral Finance school.

In attempting to explain the excess volatility found in Shiller’s work, Behavioral Finance models built in sentiment factors that would switch between optimism and pessimism with set probabilities. This would seem to explain the persistent swings in the market while it deviates from the fundamental value of the asset. The changes in pessimism to optimism or *vice versa* are modeled by a Markov switching chain is implied to be foreseeable and thus can be modeled probabilistically. It can be thought of as such: When the market is optimistic, it will remain so with probability *p* and will become pessimistic with probability 1-*p*. If it is pessimistic it will remain so with probability *q* and will become pessimistic with probability 1-*q*. This switching model allows for distinct distributions to represent change at different times. Suppose *p* is large. The market would remain persistently optimistic for a long time and would continue to bid up the price to a level above the REH price, thus explaining Shiller’s excess volatility model. 

However, there are certainly pitfalls with this approach. Behavioral economics models, as well as REH models, fail to take into account unforeseeable change. Thus, the Markov chain falls apart, as such structural change like COVID, which on average drove prices on 2 out of 3 trading days, changes the switching probabilities significantly. Thus, developments in the pandemic and factors directly influenced by the pandemic change the switching probabilities. We have already noted the correlation between the Government and Fiscal factors and the pandemic factors, but it would serve us well to revisit them. One of the main keywords found frequently throughout the Bloomberg Market Wraps were “stimulus talks” or some equivalent; this stimulus is clearly influenced directly by the pandemic, a KU factor thus we can consider the stimulus talks themselves to be KU in a way, thus their probable outcomes cannot be characterized *ex ante*. The constant back and forth on the stimulus negotiations caused the switching probabilities to continuously change throughout this period, rendering an initial model or characterization useless. Thus, while this approach more or less explains the excess volatility in theory, based on the data and the actual timeline of events, it does not adequately characterize market direction or volatility.

This brings us to our final school of thought, one that ultimately can provide the best explanation for the data we have, Knightian Uncertainty. Knight introduced a key distinction as to what uncertainty actually is: measurable uncertainty is “risk” while “true uncertainty” cannot “by any method be reduced to an objective, quantitatively defined probability”.[^4] Based on both the nature of the data as well as the timeline that the events of the time period in question followed, Knightian uncertainty certainly captures this as far as their scope is concerned. As alluded to in discussing Behavioral Finance models, the pandemic certainly could not have been characterized in terms of probability and the final decision as far the stimulus negotiations are concerned are, and I must use this word with caution, similarly uncertain. These models bound the expected value i.e. the forecasts to lie somewhere within a range that can sufficiently cover potential swings. Further this model is clearly the most rational, as previously defined. It is clear both logically and empirically that unforeseeable change occurs. To construct a model or a forecast upon a time-invariant premise would be to forego a profit-seeking opportunity which would clearly be irrational. As Knight describes, if the world indeed did not go unforeseeable change, all factors relevant to a stock price could be characterized *ex ante* then profit or loss never arises. Another point is that even in a time-fixed model, we notice a contradiction wherein if the model has undergone structural change in the past then it can be expected to do so again, thereby making a time-invariant model seem all the more irrational. Therefore, it is abundantly clear that in interpreting the data and the financial characteristics of the year 2020 as a whole, it is imperative to use an open model under the premises of Knightian Uncertainty. Given these considerations, such a model is the best candidate in explaining the data I have presented. It attributes appropriate importance to all relevant factors, fundamental, psychological, technical and unforeseeable change alike. In regard to the weight given to psychological factors, it is important to consider that we can only forecast as well as our understanding will allow us in the presence of sufficient data. In the absence of either, as it very often the case, we often regress and make decisions based on what our impulse is. This notion is very well upheld given that the majority of the psychological data captured in my interval was in conjunction with fundamentals. Thus, given the appropriate weight, we can confidently say that such factors like the pandemic and governmental and fiscal factors were powerful movers of the market this past year. 

**Conclusion**

To briefly summarize, it is apparent that the year 2020 has not only been a significant year for the markets, including stocks, cryptocurrencies, and Forex, it has been one characterized by constantly evolving unforeseeable change. The unforeseeable change that was the pandemic has gone on to impact fundamentals, and the psyches of market participants setting record levels for both the Dow and Bitcoin and exhibiting a great deal of volatility in nearly all asset markets. This pandemic has been, as shown by the regression analysis, the single greatest mover of the market this year. Given that its effects have influenced fundamental factors, the impact it has on the market has been amplified. We have shown the relative importance through frequency analysis of the main categories of movers — fundamental, psychological, technical, and KU — and have more or less been able to replicate in qualitative terms results laid out by research projects of far greater scope and magnitude conducted by Mangee and Frydman, thus lending some validity to the work that lies herein. We should continue to monitor the impact that the pandemic has, not only in our personal lives, but also the role it will play in the market in the coming months and see what new unforeseeable change will unfold. 

**Bibliography**

“Coronavirus Update: COVID-19 Likely to Cost Economy $1 Trillion during 2020, Says UN Trade Agency | | UN News.” United Nations. United Nations. Accessed December 18, 2020. https://news.un.org/en/story/2020/03/1059011. 

Nicholas Mangee. *How Novelty and Narratives Drive the Stock Market: Black Swans, Animal Spirits and Scapegoats*. Boston. Cambridge University Press. Forthcoming. 

Frank Knight. *Risk, Uncertainty, and Profit*. Boston, New York: Houghton Mifflin Company, 1921.

Frydman, Roman, Nicholas Mangee, and Josh Stillwagon. “How Market Sentiment Drives Forecasts of Stock Returns.” *Journal of Behavioral Finance*, 2020, 1–17. https://doi.org/10.1080/15427560.2020.1774769. 


[^1]: #  Coronavirus update: COVID-19 likely to cost economy $1 trillion during 2020, says UN trade agency, https://news.un.org/en/story/2020/03/1059011

    
[^2]: I have decided to treat COVID as a KU factor due to its novel nature. Upon its discovery and introduction into the global population it can certainly have been considered a KU factor. However, each subsequent update in its progression is fundamentally new and different as it is digested by the market thus changing the parameters under which the market operates and thus can be considered a KU factor.
[^3]: *How Novelty and Narratives Drive the Stock Market*. The dictionaries used to define the other terms have been borrowed from Professor Mangee.
[^4]: Knight, 1921, p.321
