# Weekly Discussions

## Data Visualization

People are not good at looking at an endless stream of numbers and seeing a pattern. However when we plot them on a graph and look at where things land it often becomes much easier to understand the macro view of the clustering or trending.

For example at work we have 1000+ data feeds coming from 200+ servers, equating to roughly 5TB/day of data ingestion. My leadership team needs to know which of these feeds are growing and if something needs to take place. They also need this information consolidated to a 3 minute conversation during a 60 minute weekly meeting.

To accomplish this I use tree maps to show the general size of one feed over another. Bar charts with trending lines are another good option for telling the story of what is happening.

The hard part is not building the charts, its making sure that the chart tells the story accurately. To build the charts you can use Power BI Desktop (easiest) or Power Query/Map/View for Excel. All are free Microsoft add-ins.  Once you point it at data you can quickly slice and dice with drag/drop features.

To tell the story correctly read "The Visual Display of Quantitative Information" by Edward R. Tufte. It's a book full of different charts and he describes why they are good or bad. Very easy read

http://classes.ninabellisio.com/GD3371/tufte.pdf has preview or buy the whole thing at http://www.amazon.com/The-Visual-Display-Quantitative-Information/dp/0961392142

## Is Amazon a Good Deal

A real world use case would be pricing of goods, services, and securities. For example I want to buy Amazon stock, assuming it is a good deal.

Software programs allow me to see that based on the last 6 months volatility the current 600$ share should be worth between 500 to 715. This range is based on determined by finding 1 standard deviation of the data set. At 2 standard deviations the range increases to 400 and 820.

Based on this information it becomes reasonable to conclude that 600 is a good deal on the stock, provided I'm willing to purchase and hold it. I think Amazon is a growing company and more likely to reach the 715 so that gives an assumed return of 20%/115$ (715- 600), ignoring commissions.

However using the variance and standard deviations the software says that this will likely take 1 year, making the quarterly return 5%.

Now we the question becomes is there other options which offer a higher return than 5%, with a similar risk level?  If not, then this is a good deal.
