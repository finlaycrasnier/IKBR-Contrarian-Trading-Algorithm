# IKBR-Contrarian-Trading-Algorithm
A small contrarian trading algorithm I created whilst learning from a Udemy equity trading course. The strategy revolves around purchasing stocks which have a relatively 'low' daily return, and shorting stocks that have a relatively 'high' daily return in hope that they will return to their average value in the following days. Once this occurs, they can be sold for a profit. Comments explaining the programming and strategy in more detail be found in the Python file.  

For personal development, I challenged myself to think of some potential problems when using such a strategy. I also thought of some potential improvements that could alleviate some of these problems, or improve the efficiency of the code. I may amend these once I progress further into my course.

## Problems with the strategy

- No fundamental influencers are included; a stock may rapidly rise because of overwhelmingly positive financial reports or media coverage. These stocks may not revert to their average value.
- No purchase variance between the most significant outlier stocks VS standard outlier stocks
- Overall market picture is not viewed / lack of safety net; index could be rapidly growing and we will continue to short stocks

## Improvements to the strategy

- Link to company financial reporting to get a better sense if the change is technical (in which case our algorithm is suitable) or fundamental
- Create a scaled purchase amount; the most extreme 'high' return stocks should command a larger purchase amount
- Create a dynamic amount of buy/short stocks; in a rising market, we will trade more declining stocks
- Adjust the algorithm to purchase a value amount (fractional shares) rather than multiples of shares, allowing Dollar Cost Averaging to be utilised

## Improvements to the algorithm

- Create a user input prompt that allows them to choose how many shares, how many top/bottom stocks and which index to use
- Convert the algorithm into a script that automatically runs just before the market close
- Add a 'safety' net; some stocks may only increase marginally (e.g. by 0.000001%), but may appear 'high' if the overall index is performing poorly

## Concluding thoughts

Overall, I am pretty happy with how the project turned out. I think it's a pretty good start to my learning, and I look forward to seeing how I can improve in the future.



