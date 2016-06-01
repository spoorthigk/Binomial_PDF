# Binomial_PDF
%Plotting a Binomial PDF graph in MATLAB with given number of samples as 50 with the probability of occurrence as 0.4

N=50;
p=0.4; 
for n=0:1:50
b=(factorial(N))/((factorial(n))*(factorial(N-n)))*((p^n)*(1-p)^(N-n)); 
stem(n,b); 
hold on;
end
xlabel('n');
ylabel('discrete pdf');
title(' Binomial');
