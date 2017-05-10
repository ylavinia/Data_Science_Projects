The thanksgiving.csv file contains 1058 responses to an online survey about what Americans eat for Thanksgiving dinner. Each survey respondent was asked questions about what they typically eat for Thanksgiving, along with some demographic questions, like their gender, income, and location. This dataset will allow us to discover regional and income-based patterns in what Americans eat for Thanksgiving dinner.

The dataset has 65 columns, and 1058 rows. Most of the column names are questions, and most of the column values are string responses to the questions. Most of the columns are categorical, as a survey respondent had to select one of a few options. For example, one of the first column names is What is typically the main dish at your Thanksgiving dinner?. The potential responses are:

Turkey
Other (please specify)
Ham/Pork
Tofurkey
Chicken
Roast beef
I don't know
Turducken
Most of the columns follow the same question/response format as the above. There are also quite a few NaN values in the columns, which occurred when a survey respondent didn't fill out a question because they didn't want to, or it didn't apply to them.

Here are the first few rows of the dataset:

RespondentID	Do you celebrate Thanksgiving?	What is typically the main dish at your Thanksgiving dinner?	What is typically the main dish at your Thanksgiving dinner? - Other (please specify)	How is the main dish typically cooked?	How is the main dish typically cooked? - Other (please specify)	What kind of stuffing/dressing do you typically have?	What kind of stuffing/dressing do you typically have? - Other (please specify)	What type of cranberry saucedo you typically have?	What type of cranberry saucedo you typically have? - Other (please specify)	...	Have you ever tried to meet up with hometown friends on Thanksgiving night?	Have you ever attended a "Friendsgiving?"	Will you shop any Black Friday sales on Thanksgiving Day?	Do you work in retail?	Will you employer make you work on Black Friday?	How would you describe where you live?	Age	What is your gender?	How much total combined money did all members of your HOUSEHOLD earn last year?	US Region
0	4337954960	Yes	Turkey	NaN	Baked	NaN	Bread-based	NaN	None	NaN	...	Yes	No	No	No	NaN	Suburban	18 - 29	Male	75,000 to 99,999	Middle Atlantic
1	4337951949	Yes	Turkey	NaN	Baked	NaN	Bread-based	NaN	Other (please specify)	Homemade cranberry gelatin ring	...	No	No	Yes	No	NaN	Rural	18 - 29	Female	50,000 to 74,999	East South Central
2	4337935621	Yes	Turkey	NaN	Roasted	NaN	Rice-based	NaN	Homemade	NaN	...	Yes	Yes	Yes	No	NaN	Suburban	18 - 29	Male	0 to 9,999	Mountain
3	4337933040	Yes	Turkey	NaN	Baked	NaN	Bread-based	NaN	Homemade	NaN	...	Yes	No	No	No	NaN	Urban	30 - 44	Male	$200,000 and up	Pacific
4	4337931983	Yes	Tofurkey	NaN	Baked	NaN	Bread-based	NaN	Canned	NaN	...	Yes	No	No	No	NaN	Urban	30 - 44	Male	100,000 to 124,999	Pacific
5 rows × 65 columns

The following are descriptions of some of the most important columns:

RespondentID -- a unique ID of the respondent to the survey.
Do you celebrate Thanksgiving? -- a Yes/No reponse to the question.
How would you describe where you live? -- responses are Suburban, Urban, and Rural.
Age -- resposes are one of several categories, such as 18-29, and 30-44.
How much total combined money did all members of your HOUSEHOLD earn last year? -- one of several categories, such as $75,000 to $99,999.
