# Go-Daddy.1
Interactive Shiny app built in R to analyze GoDaddy’s microbusiness survey data. Visualizes trends in capital investment, customer satisfaction, website traffic, and market reach to support strategic decisions and optimize service offerings.

Steps involved:

-Import and clean raw survey data from Excel in RStudio

-Understand and map survey responses using provided documentation

-Explore key business questions related to investment, website traffic, customer satisfaction, and market reach

-Build a responsive Shiny dashboard with 4–6 components (graphs/tables) based on user input

-Submit reproducible, annotated R code and a two-page summary highlighting data cleaning steps and stakeholder-relevant insights

Question 1: How do capital investment patterns differ across industries, and what insights can be gained for strategic decision-making?
For the first question, I used business categories (Column 5c), which specify the industry in which the customer operates, and the range of capital investment (Column 5d), named as Values1 and Values2, respectively. I merged them with the dataset “data.” In the business category column, any missing values marked as (-7) were labeled as “Missing.” For the range of capital investment column, I renamed some categories as “Don’t know,” “Prefer not to answer,” and “Missing” based on the value descriptions in the dataset. The visualization I created is an interactive graph that has a drop-down option that lets users filter by business category and allows users to analyze how many customers invested within different capital ranges. For businesses with lower capital investment, like startups, GoDaddy can offer affordable shared hosting and easy website builders to help them establish an online presence. Businesses with higher capital investment like tech firms may require dedicated servers, cloud hosting, and advanced security to handle larger operations. Industry-specific needs play a role too—consulting firms may benefit from professional email and client management tools, while e-commerce businesses require fast servers, secure payment gateways, and personalized marketing tools to enhance customer experience and sales.
![image](https://github.com/user-attachments/assets/56014f78-7954-47f1-b549-00394a35754a)

Question 2: How can GoDaddy optimize its services for different business categories based on website traffic patterns and customer demand?
For the second question, I analyzed the website traffic businesses receive by using business category (Column q5) and the actual count of website visitors (Column q6). I created a heatmap where the x-axis represents different business categories-commercial, civic, etc; and the color intensity indicates the density of customers based on the number of website visitors. This heatmap provides insights into business categories where GoDaddy could optimize its services. Commercial websites show the highest demand, requiring high-performance servers, e-commerce integrations, and marketing tools. Personal websites indicate a need for affordable hosting and easy website builders. Meanwhile other categories have lower demand and could benefit from low-cost shared hosting and local SEO tools. 
![image](https://github.com/user-attachments/assets/da35b407-e21b-495b-8cca-bde5b5205f65)


Question 3: How can GoDaddy improve customer retention and satisfaction based on hosting duration trends and rating insights?
For the third question, I examined customer ratings and website hosting duration to assess satisfaction trends. Customers rate the company based on how likely they are to recommend it to others, while the duration of website hosting is categorized into different time ranges (e.g., less than 1 year, 1-3 years, etc.). To visualize this, I created a stacked bar graph, where users can select a specific rating (e.g., 8). The graph then shows the percentage of customers who rated 8 or above (labeled as “Above”) and those who rated below 8 (labeled as “Below”), categorized by the number of years they have been hosting their website. This analysis helps a web hosting company identify customer satisfaction trends based on hosting duration. While onboarding experiences may be strong, long-term customers often face issues with service consistency, pricing, or outdated plans. To address this, Go can enhance customer engagement through loyalty programs and feature upgrades to retain mid-term users. These could help to optimize retention strategies, introduce targeted incentives, and refine service offerings to ensure customer loyalty and reduce mid-term churn

![image](https://github.com/user-attachments/assets/6f004808-d162-418f-bf7b-cc6680bd6f90)

Question 4: How can GoDaddy tailor its services to different business operation modes and audience scopes to optimize market reach?
For the fourth question, I focused on analyzing the mode of business operation and the audience scope. I used the mode of business (Column q5b), which indicates whether a business operates online, offline, or in a hybrid model, and the scope of their audience, which describes whether they target customers at the neighborhood, city, or state level. The visualization created for this question shows how many businesses operate in each mode and how their audience scope varies, helping them understand the relationship between business operations and market reach. This analysis helps web hosting companies understand how business mode influences market reach, showing that most online businesses target country-wide or global audiences. This highlights the importance of scalable hosting solutions, where global and country-wide businesses require high-performance servers, CDN integration, multi-language support, and advanced security for seamless user experiences, while local businesses at the neighborhood or city level benefit more from affordable hosting, localized SEO, and small business website packages.
![image](https://github.com/user-attachments/assets/e030642e-4591-49bb-b692-9378d5529c19)
