#Project work
#scatter plot using x1 and y1
plot(x1, y1, main = "X vs Y", xlab = 'Xnumbers', ylab = 'Ynumbers', 
     mtext(side = 3, text = paste(cor(x1, y1))), col = 'purple', pch = 19)

#calculating correlation coefficient
cor(x1, y1, method = 'pearson')

#constructing histogram
hist(x1, col = "blue", xlab = "Xnumbers", ylab = "Frequency",
     main = "Histogram(x1)")

#constructing boxplots
boxplot(y1, xlab = 'y1',ylab = 'Frequency')
boxplot(x1, y1)
boxplot(x1, y1, horizontal = TRUE)

par(mfrow=c(2,1))
boxplot(x1, y1)
hist(x1)

par(mfrow=c(1,2))
boxplot(x1, y1, main = 'Boxplot(x1,y1')
hist(x1)
