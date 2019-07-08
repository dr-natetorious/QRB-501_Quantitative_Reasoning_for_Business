# Weekly Discussions

## Assets - Liability = Equity

I'll admit that I stared at this for a minute or two, due to the way the book worded the formula.

A = L +E

That didn't make sense, why would I be totaling liability (debt) with equity (value). Though using a bit of 2nd grade math it becomes

E (value) = Assets (stuff) - Liability (debt)

Assets are: chairs, buildings, intellectual property, etc.

Liabilities are: salaries, mortgages, debt, etc.

Equity is: value of accounted thing.

## LendingClub.com Dumped into Excel

I got an email about investing in peer-to-peer lending. Basically the idea is that you take a large loan, then break it up into 25$ chunks. Each chunk is sold to a different person, so if the loan defaults you are only out 25$/share.

They also claim that if you invest across 100+ of these notes, then through diversity it is possible to have "relatively" safe and predictable returns. However the hard part is figuring out which ones to pick. So I wrote a script to download all active loan requests [into Excel](lendingclub.csv), and loaded the results [into Power BI](Week%204%20-%20Lending%20Club%20PowerBI%20Example.zip).

The challenge with Lending Club, is that most of their loans are for low credit scores trying to refinance debt. This has an upside but presents significant risk to the investor. From spot picking several of these refi have 50+ lines of credit, which suggests extreme debt to equitity ratios.

Based on the interactive charts, I think that my core filter would be:

High FICO Score (720+)
Loan Purpose: House, Home Improvement, Small Business
Term: 36 months
Loan Amount: < 35k (web site max limit = 35k)
These customers tend to be people with a history of repaying their debt, and are looking for short term loans. This would suggest they are entering the agreement in good faith.

Compared to those with purpose of car purchase; which are willing to accept a 24% interest rate over 5 years. These people are nuts as most car dealerships are offering <= 10%; which suggests those are bad debt.

The web site also provides statistics that the longer the loan the more likely to default. Since there are only 36/60 month options, it would statistically mean 36 are better pay; even at the lower APR.

The last criteria is the amount of the loan. Since the web site supports a maximum of 35k, this means anyone requesting 35k is likely looking for max debt. By putting a threshold of 85/90% it would filter out a significant portion of bad debtors.
