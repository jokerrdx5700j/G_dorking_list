# Google Dorking Commands

## Basic Operators
1. `"search term"` - Searches for the exact phrase.
2. `site:example.com` - Searches within a specific site.
3. `filetype:pdf` - Searches for files of a specific type.
4. `intitle:"keyword"` - Searches for pages with a specific keyword in the title.
5. `inurl:"keyword"` - Searches for URLs containing a specific keyword.

## Advanced Operators
6. `cache:example.com` - Shows the cached version of a webpage.
7. `link:example.com` - Finds links to a specific website.
8. `related:example.com` - Finds sites related to a specific website.
9. `info:example.com` - Provides information about a particular website.
10. `allintext:keyword` - Searches for pages with all terms in the body text.

## Security and Vulnerability Searching
11. `intext:"password"` - Searches for pages containing the word "password".
12. `inurl:login` - Searches for login pages.
13. `inurl:admin` - Searches for admin login pages.
14. `inurl:wp-login.php` - Searches for WordPress login pages.
15. `filetype:sql` - Searches for SQL files potentially containing sensitive data.

## File Searches
16. `filetype:xls` - Searches for Excel files.
17. `filetype:doc` - Searches for Word documents.
18. `filetype:ppt` - Searches for PowerPoint presentations.
19. `filetype:xml` - Searches for XML files.
20. `filetype:csv` - Searches for CSV files.

## Indexing and Data Searching
21. `site:gov` - Searches government websites.
22. `site:edu` - Searches educational institution websites.
23. `site:org` - Searches non-profit organization websites.
24. `intext:"credit card"` - Searches for pages containing "credit card" information.
25. `intext:"social security"` - Searches for social security numbers.

## Combine Searches
26. `"search term" OR "alternative term"` - Searches for either term.
27. `"search term" AND "other term"` - Searches for results containing both terms.
28. `"search term" -exclude_term` - Searches for results excluding a specific term.
29. `"search term" AROUND(3) "other term"` - Searches for terms within a certain distance from each other.
30. `"search term" * "other term"` - Searches for results with anything in between.

## Location-Based Searches
31. `"keyword" inurl:location` - Searches for pages containing a location.
32. `"keyword" site:.uk` - Searches for UK sites.
33. `"keyword" site:.ca` - Searches for Canadian sites.
34. `"keyword" site:.au` - Searches for Australian sites.
35. `"keyword" site:.de` - Searches for German sites.

## Miscellaneous Searches
36. `"keyword" define:` - Finds definitions for a keyword.
37. `"keyword" movie:` - Searches for movies related to the keyword.
38. `"keyword" recipe:` - Searches for recipes related to the keyword.
39. `"keyword" news:` - Searches for news related to the keyword.
40. `"keyword" sports:` - Searches for sports news related to the keyword.

## Custom Finance Searches
41. `"investing" filetype:pdf` - Searches for investing PDF guides.
42. `"stock market" intext:"crash"` - Looks for stock market crash discussions.
43. `"financial report" filetype:xls` - Searches for financial Excel reports.
44. `"budget" filetype:doc` - Searches for budgeting documents.
45. `"financial analysis" site:edu` - Looks for academic financial analysis papers.

## Academic Searches
46. `"thesis" filetype:pdf` - Searches for academic theses.
47. `"research paper" site:edu` - Searches for educational research papers.
48. `"dissertation" filetype:doc` - Searches for doctoral dissertations.
49. `"conference paper" filetype:ppt` - Searches for conference presentations.
50. `"journal article" filetype:pdf` - Searches for academic articles.

## Creative Content Searches
51. `"music lyrics"` - Searches for song lyrics.
52. `"art portfolio"` - Searches for artist portfolios.
53. `"graphic design" filetype:pdf` - Searches for PDF files related to graphic design.
54. `"photography" site:500px.com` - Searches for specific photography sites.
55. `"architecture" blueprint filetype:jpg` - Searches for blueprint images.

## Employment Searches
56. `"Job Title" site:linkedin.com` - Searches for job postings on LinkedIn.
57. `"resume" filetype:pdf` - Searches for PDF resumes.
58. `"interview tips"` - Searches for interview tips resources.
59. `"career advice"` - Searches for career advice articles.
60. `"salary" site:glassdoor.com` - Searches for salary information.

## Code and Development Searches
61. `"code samples" filetype:py` - Searches for Python code samples.
62. `"API documentation"` - Searches for API documentation.
63. `"web development" site:github.com` - Searches for GitHub web development projects.
64. `"open-source project" filetype:zip` - Searches for downloadable open-source projects.
65. `"software development" inurl:blog` - Searches for software development blogs.

## Government & Legal Searches
66. `"lawsuit" filetype:pdf` - Searches for PDF files related to lawsuits.
67. `"legislation" site:gov` - Searches for legal documents on government websites.
68. `"public records" filetype:csv` - Searches for public records in CSV format.
69. `"court case" site:uscourts.gov` - Searches for federal court cases.
70. `"legal advice"` - Searches for legal advice articles.

## Technology Searches
71. `"gadget review"` - Searches for reviews on gadgets.
72. `"tech news"` - Searches for technology news articles.
73. `"programming languages"` - Searches for information on programming languages.
74. `"hardware specifications"` - Searches for hardware specifications.
75. `"software updates"` - Searches for recent software updates.

## Health & Wellness Searches
76. `"fitness tips"` - Searches for fitness-related articles.
77. `"diet plans"` - Searches for weight loss diet plans.
78. `"hospital information" site:gov` - Searches for government hospital resources.
79. `"medical research" filetype:pdf` - Searches for medical research papers.
80. `"healthcare policy"` - Searches for healthcare policy discussions.

## Travel Searches
81. `"travel tips"` - Searches for travel tips.
82. `"flight deals"` - Searches for flight deals and discounts.
83. `"hotel reviews"` - Searches for hotel reviews.
84. `"travel blogs"` - Searches for travel blogs.
85. `"tourist attractions"` - Searches for popular tourist attractions.

## Real Estate Searches
86. `"homes for sale" site:realestate.com` - Searches for homes for sale.
87. `"rental properties" site:apartmentfinder.com` - Searches for rental properties.
88. `"real estate market analysis" filetype:pdf` - Searches for PDF real estate analyses.
89. `"property investment tips"` - Searches for property investment advice.
90. `"mortgage rates"` - Searches for current mortgage rates.

## Personal Development Searches
91. `"self-help books"` - Searches for self-help book suggestions.
92. `"motivational quotes"` - Searches for motivational quotes.
93. `"goal setting strategies"` - Searches for goal-setting articles.
94. `"time management tips"` - Searches for time management techniques.
95. `"mindfulness practices"` - Searches for mindfulness and meditation tips.

## Environmental Searches
96. `"climate change research" filetype:pdf` - Searches for climate change studies.
97. `"renewable energy technologies"` - Searches for renewable energy articles.
98. `"environmental policy" site:gov` - Searches for government environmental policies.
99. `"conservation efforts"` - Searches for conservation-related initiatives.
100. `"sustainable practices"` - Searches for sustainability practices in various fields.


## Additional Commands

### Business and Finance
101. `"investment strategies"` - Searches for investment advice.
102. `"credit score tips"` - Searches for ways to improve credit scores.
103. `"business plan templates" filetype:doc` - Searches for business plan templates.
104. `"market research" filetype:pdf` - Searches for market research reports.
105. `"financial literacy"` - Searches for financial literacy resources.

### Social Media and Marketing
106. `"social media trends"` - Searches for information about social media trends.
107. `"influencer marketing"` - Searches for tips on influencer marketing.
108. `"blogging tips"` - Searches for blogging advice.
109. `"SEO strategies"` - Searches for search engine optimization strategies.
110. `"content marketing"` - Searches for content marketing techniques.

### Parenting and Family
111. `"parenting tips"` - Searches for parenting advice.
112. `"newborn care"` - Searches for resources on caring for newborns.
113. `"educational activities for kids"` - Searches for educational activities.
114. `"family vacation ideas"` - Searches for family-friendly vacation ideas.
115. `"teenage issues"` - Searches for advice on dealing with teenage issues.

### Science and Technology
116. `"quantum computing"` - Searches for information on quantum computing.
117. `"artificial intelligence research" filetype:pdf` - Searches for AI research papers.
118. `"blockchain technology"` - Searches for resources on blockchain.
119. `"space exploration"` - Searches for space exploration articles.
120. `"biotechnology"` - Searches for biotechnology advancements.

### Lifestyle and Hobbies
121. `"cooking recipes"` - Searches for various cooking recipes.
122. `"hiking trails"` - Searches for popular hiking trails.
123. `"DIY projects"` - Searches for do-it-yourself project ideas.
124. `"home improvement tips"` - Searches for home renovation advice.
125. `"gardening tips"` - Searches for gardening advice.

### Arts and Culture
126. `"art exhibitions"` - Searches for art exhibitions.
127. `"literary reviews"` - Searches for reviews of literature.
128. `"music concerts"` - Searches for information on music concerts.
129. `"film reviews"` - Searches for film critiques.
130. `"theater performances"` - Searches for theater events.

### Technology and Gadgets
131. `"latest smartphones"` - Searches for information on latest smartphones.
132. `"computer hardware reviews"` - Searches for computer hardware assessments.
133. `"digital cameras"` - Searches for latest digital cameras.
134. `"software comparisons"` - Searches for comparisons of software products.
135. `"tech gadgets"` - Searches for new technology gadgets.

### Fitness and Health
136. `"workout plans"` - Searches for exercise plans.
137. `"nutrition guides"` - Searches for nutrition information.
138. `"mental health resources"` - Searches for mental health support.
139. `"wellness tips"` - Searches for general wellness advice.
140. `"yoga practices"` - Searches for yoga techniques.

### Travel and Adventure
141. `"adventure travel"` - Searches for adventure travel ideas.
142. `"best travel destinations"` - Searches for top travel locations.
143. `"budget travel tips"` - Searches for travel on a budget.
144. `"road trips"` - Searches for popular road trip routes.
145. `"cultural experiences"` - Searches for cultural travel experiences.

### Personal Finance
146. `"saving strategies"` - Searches for ways to save money.
147. `"retirement plans"` - Searches for retirement planning resources.
148. `"debt relief options"` - Searches for information on relieving debt.
149. `"credit repair tips"` - Searches for repairing credit scores.
150. `"investing basics"` - Searches for beginner investing information.

### Food and Dining
151. `"local restaurants"` - Searches for restaurants in a specific area.
152. `"food truck events"` - Searches for food truck gatherings.
153. `"cooking classes"` - Searches for cooking courses available.
154. `"ethnic cuisines"` - Searches for different types of ethnic foods.
155. `"wine tasting events"` - Searches for wine tasting opportunities.

### Home and Garden
156. `"interior design ideas"` - Searches for home decor inspirations.
157. `"landscaping tips"` - Searches for landscaping advice.
158. `"home organization"` - Searches for tips on organizing the home.
159. `"sustainable gardening"` - Searches for eco-friendly gardening practices.
160. `"real estate trends"` - Searches for current real estate trends.

### Career Development
161. `"professional networking"` - Searches for networking opportunities.
162. `"career advancement tips"` - Searches for ways to advance in a career.
163. `"online courses"` - Searches for available online courses.
164. `"skill development"` - Searches for skills development resources.
165. `"mentorship opportunities"` - Searches for mentorship programs.

### History and Culture
166. `"historical research papers" filetype:pdf` - Searches for historical studies.
167. `"cultural heritage"` - Searches for cultural preservation topics.
168. `"art history"` - Searches for art movements and history.
169. `"significant historical events"` - Searches for major historical occurrences.
170. `"ethnic studies"` - Searches for information on various ethnic groups.

### Technology and Innovations
171. `"latest tech news"` - Searches for up-to-date technology news.
172. `"gadget reviews"` - Searches for reviews on the latest gadgets.
173. `"software updates"` - Searches for information about newly released software updates.
174. `"app comparisons"` - Searches for comparisons of mobile applications.
175. `"tech career paths"` - Searches for information on technology-related careers.

### Sports and Recreation
176. `"team schedules"` - Searches for sports team schedules.
177. `"fitness challenges"` - Searches for competitive fitness events.
178. `"sports betting tips"` - Searches for tips on sports betting.
179. `"outdoor sports activities"` - Searches for outdoor sporting events.
180. `"eSports competitions"` - Searches for eSports tournament information.

### Education and Learning
181. `"online learning platforms"` - Searches for platforms offering online education.
182. `"study tips"` - Searches for effective study methodologies.
183. `"learning resources for students"` - Searches for educational materials.
184. `"home schooling tips"` - Searches for advice on home schooling.
185. `"curriculum development"` - Searches for curriculum planning resources.

### Arts and Crafts
186. `"art supplies"` - Searches for local craft stores.
187. `"craft tutorials"` - Searches for crafting instruction videos.
188. `"art workshops"` - Searches for available art classes.
189. `"DIY home decor"` - Searches for do-it-yourself decor projects.
190. `"community art projects"` - Searches for local art initiatives.

### Community and Society
191. `"volunteer opportunities"` - Searches for local volunteering possibilities.
192. `"community events"` - Searches for happenings in a community.
193. `"non-profit organizations"` - Searches for local non-profits.
194. `"social activism"` - Searches for information about social justice movements.
195. `"support groups"` - Searches for various support communities.

### Environmental Issues
196. `"climate change impacts"` - Searches for effects of climate change.
197. `"sustainability practices"` - Searches for sustainable living advice.
198. `"wildlife conservation"` - Searches for wildlife protection initiatives.
199. `"eco-friendly products"` - Searches for green product alternatives.
200. `"pollution solutions"` - Searches for ways to combat pollution.

