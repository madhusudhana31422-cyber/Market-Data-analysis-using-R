# Market-Data-analysis-using-R

This is a beginner-level R programming project created to practice data frames and basic data analysis.

🔹 What I did in this project:
Created a data frame with fruit names and prices
Used head() and str() to understand data structure
Applied conditional logic (ifelse) to classify prices as High / Low budget
Filtered data based on conditions
Sorted data by price in descending order

🔹 Concepts Used:
Data Frames
Column operations
Conditional statements
Data filtering
Sorting data in R

🔹CODE
market<-data.frame(
  name=c("Apple","Orange","Graphs","Mango"),
  price=c(130,200,60,120)
)
market

head(market)
str(market)
which(market$price>80)

market$budjet<-ifelse(market$price>=100,"High","low")
market

market[market$budjet=="High",]
market[order(-market$price),]
