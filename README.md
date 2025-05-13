# ematm0061-lab-5-solved
**TO GET THIS SOLUTION VISIT:** [EMATM0061 Lab 5 Solved](https://www.ankitcodinghub.com/product/ematm0061-lab-5-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93042&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EMATM0061 Lab 5 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
This document describes your fifth assignment for Statistical Computing and Empirical Methods (Unit EMATM0061) on the MSc in Data Science. Before starting the assignment it is recommend that you first watch video lectures 11 and 12.

You are encouraged to discuss these questions with your colleagues.

Begin by creating an Rmarkdown document with html output. You are not expected to hand in this piece of work, but it is a good idea to get used to using Rmarkdown.

Several optional extra questions have also been included. These are marked by stars (‘*“). It is recommended that you first complete all unstarred questions before proceeding through the starred questions. Do not be concerned if you do not have time to complete the starred questions!

1 Expectation and variance of a discrete random variable

Suppose that α,β ∈ [0,1] with α+β ≤ 1 and let X be a discrete random variable with with distribution supported on {0, 1, 5}. Suppose that P (X = 1) = α and P (X = 5) = β and P (X ∈/ {0, 1, 5}) = 0.

What is the probability mass function pX : S → [0,1] for X? What is the expectation of X?

What is the variance of X?

2 Simulating data with the uniform distribution

We shall now use the uniform distribution to simulate data from the discrete random variable discussed in the previous question. A uniformly distributed random variable U is a continuous random variable with probability density function

􏰕1 ifx∈[0,1] pU (x) = 0 otherwise.

Show that for any region pair of numbers a,b ∈ R with 0 ≤ a ≤ b ≤ 1 we have P(U ∈ [a, b]) = b − a. 1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Now let’s return to the discrete random variable discussed in the previous question in which P (X = 1) = α and P (X = 5) = β and P (X = 0) = 1 − α − β. First consider the case in which α = β = 0.25. You can generate a sequence of i.i.d. copies X1 , . . . , Xn of X as follows:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
set.seed(0)

n&lt;-1000

<pre>sample_X&lt;-data.frame(U=runif(n))%&gt;%
  mutate(X=case_when(
</pre>
<pre>    (0&lt;=U)&amp;(U&lt;0.25)~1,
    (0.25&lt;=U)&amp;(U&lt;0.5)~5,
    (0.5&lt;=U)&amp;(U&lt;=1)~0))%&gt;%
</pre>
pull(X)

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Why does this sample_X correspond to a sequence of i.i.d. copies X1, . . . , Xn of X where P (X = 1) = α and P (X = 5) = β and P (X = 0) = 1 − α − β with α = β = 0.25?

Now create a function called sample_X_015() which takes as inputs α, β and n and outputs a sample X1 , . . . , Xn of independent copies of X where P (X = 1) = α and P (X = 5) = β and P (X = 0) = 1 − α − β.

Next take α = 1/2 and β = 1/10, and use your function sample_X_015() to create a sample of size n = 10000, of the form X1, . . . , Xn consisting of independent copies X for each value of β. What is the sample average of X1, . . . , Xn? How does this compare with E(X)? Use your understanding of the law of large numbers to explain this behaviour.

In addition, compute the sample variance of X1 , . . . , Xn and compare with Var(X ).

Now take α = 1/10 and vary β in increments of 0.01 from 0 to 9/10, using your function sample_X_015() to create a sample of size n = 100, X1, . . . , Xn consisting of independent copies X for each value of β. Create a plot of the sample averages as a function of β.

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
3 The Gaussian distribution

Write out the probability density function of a Gaussian random variable with mean μ and standard deviation σ &gt; 0.

Use the help function to look up the following four functions: dnorm(), pnorm(), qnorm() and rnorm().

Generate a plot which displays the probability density function for three Gaussian distributions X1 ∼ N(μ1,σ12), X2 ∼N(μ2,σ2)andX3 ∼N(μ2,σ32)withμ1 =μ2 =μ3 =1andvariancesσ12 =1,σ2 =2andσ32 =3. Your plot should look something like this:

</div>
</div>
<div class="layoutArea">
<div class="column">
0.4

0.3

0.2

0.1

0.0

</div>
<div class="column">
Variance 1

2 3

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Density

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
−4 −2 0 2 4 6

x

</div>
</div>
<div class="layoutArea">
<div class="column">
Generate a corresponding plot for the cumulative distribution function for three Gaussian distributions X1 ∼ N(μ1,σ12), X2 ∼ N(μ2,σ2) and X3 ∼ N(μ2,σ32) with μ1 = μ2 = μ3 = 1 and variances σ12 = 1, σ2 = 2 and σ 32 = 3 .

Next generate a plot for the quantile function for the same three Gaussian distributions. Describe the relationship between the quantile function and the cumulative distribution function.

(*) Recall that for a random variable X : Ω → R is said to be Gaussian with expectation μ and variance σ2 (X ∼ N(μ,σ2) if for any a,b ∈ R we have

􏰜b 1 −1(z−μ)2 P(a≤X≤b)= √e2 σ dz.

a σ 2π

Suppose Z ∼ N (0, 1) is a Gaussian random variable. Take α,β ∈ R and let W : Ω → R be the random variable given by W = αZ+β. Apply a change of variables to show that W is a Gaussian random variable with expectation β and variance α2.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
Note: If you are short on time you can simply take this fact as given and move onto the next part of the question.

Now use rnorm() generate a random independent and identically distributed sequence Z1, · · · , Zn ∼ N (0, 1) so that each Zi ∼ N (0, 1) has standard Gaussian distribution with n = 100. Make sure your code is reproducible by using the set.seed() function. Store your random sample in a vector called “standardGaussianSample”.

Use your existing sample stored in standardGaussianSample to generate a sample of size n of the form Y1, · · · , Yn ∼ N (1, 3) with expectation μ = 1 and population variance σ2 = 3. Store your second sample in a vector called mean1Var3GaussianSampleA.The i-th observation in the sample mean1Var3GaussianSampleA should be of the form Yi = α · Zi + β, for appropriately chosen α,β ∈ R, where Zi is the i-th observation in the sample standardGaussianSample.

Reset the random seed to the same value as before using the set.seed() function and generate an i.i.d. sample of the form Y1 , · · · , Yn ∼ N (1, 3) using the rnorm() function. Store this sample in a vector called mean1Var3GaussianSampleB. Compare the vectors mean1Var3GaussianSampleA and mean1Var3GaussianSampleB.

Now generate a graph which includes both a kernel density plot for your sample mean1Var3GaussianSampleA and the population density (the probability density function) generated using dnorm(). You can also include two vertical lines which display both the population mean and the sample mean. You may want to use the geom_density() and geom_vline() functions. Your plot should something like the following:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
0.2

0.1

0.0

</div>
</div>
<div class="layoutArea">
<div class="column">
Legend

Population density

Sample kernel density Population mean Sample mean

</div>
</div>
<div class="layoutArea">
<div class="column">
−4 −2 0 2 4 6

x

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Density

</div>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
4 The Binomial distribution and the central limit theorem

Two important discrete distributions are the Bernoulli distribution and the Binomial distribution. We say that a random variable X has Bernoulli distribution with parameter p ∈ [0, 1] if P(X = 1) = p and P(X = 0) = 1 − p. This is often abbreviated as X ∼ B(p).

Given n ∈ N and p ∈ [0, 1], we say that a random variable Z has Binomial distribution with parameters n and p if Z = X1 + ··· + Xn where Xi ∼ B(p) and X1,··· ,Xn are independent and identically distributed. This is often abbreviated as Z ∼ Binom(n, p).

(Q) Compute the expectation and variance of Z ∼ Binom(n, p). You may want to make use of following two useful facts:

􏰃􏰖k 􏰄􏰖k

1. Given any sequence of random variables W1, · · · , Wk we have E i=1 Wi = i=1 E (Wi).

2. Given independent random variables W ,··· ,W we have Var􏰃􏰖k W 􏰄 = 􏰖k Var(W ). 1 k i=1i i=1 i

Is it always true that Var􏰃􏰖k W 􏰄 = 􏰖k Var(W ), even if W ,··· ,W are not independent? i=1i i=1 i 1 k

The function dbinom() in R allows us to compute the probability mass function of a Binomial random variable Z ∼ Binom(n, p). By taking x ∈ {0, 1, . . . , n} size=n and prob=p as arguments, the function dbinom(x,size=n,prob=p) will return the probability mass function pZ(x) = P(Z = x) evaluated at x. You can run ?dbinom in the R console to find out more.

Consider the case where n = 50 and p = 7/10. Use the dbinom() to generate a dataframe called binom_df with two columns – x and pmf. The first column contains the numbers {0,1,…,50} inclusive. The second column gives the corresponding value of the probability mass function pZ(x) = P(Z = x) with Z ∼ Binom(50,7/10). Use the head() function to observe the first 3 rows as your data frame. The result should look as follows:

##x pmf ## 1 0 7.178980e-27 ## 2 1 8.375477e-25 ## 3 2 4.787981e-23

The function dnorm() in R allows us to compute the probability density function of a Gaussian random variable W ∼ N(μ,σ2) with expectation μ and variance σ2. By taking x ∈ R, mean=mu and sd=sigma as arguments, the function dnorm(x,mean=mu,sd=sigma) will return the probability density function fW (x) for W ∼ N (μ, σ2), evaluated at x. You can run ?rnorm in the R console to find out more.

We shall consider a case where μ = 50 · 0.7 and σ = 􏰝50·0.7·(1−0.7). Use the rnorm() to gener- ate a dataframe called norm_df with two columns – x and pdf. The first column contains the numbers {0, 0.01, 0.02, 0.03, . . . , 49.99, 50}. The second column gives the corresponding value of the probability den- sity function fW (x) with W ∼ N (5, 7/10). Use the head() function to observe the first 3 rows as your data frame. Your result should look as follows:

<pre>##      x          pdf
## 1 0.00 5.707825e-27
## 2 0.01 5.901264e-27
## 3 0.02 6.101201e-27
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Next, use the following code to create a plot which compares the probability density for your Gaussian distribution W ∼ N(μ,σ2) where μ = n·p and σ = 􏰝n·p(1−p) and the probability mass function for your Binomial distribution Z ∼ Binom(n, p).

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>colors&lt;-c("Gaussian pdf"="red", "Binomial pmf"="blue")
fill&lt;-c("Gaussian pdf"="white", "Binomial pmf"="white")
</pre>
ggplot()+labs(x=”x”,y=”Probability”)+theme_bw()+ geom_line(data=gaussian_df, aes(x,y=pdf,color=”Gaussian pdf”),size=2)+

# create plot of Gaussian density geom_col(data=binom_df,

<pre>                  aes(x=x,y=pmf,color="Binomial pmf",fill="Binomial pmf"))+
  scale_color_manual(name = "", values=colors)+
</pre>
<pre>  scale_fill_manual(name = "", values=fill)+
  xlim(c(20,50))
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
0.125

0.100

0.075

0.050

0.025

0.000

</div>
<div class="column">
Gaussian pdf Binomial pmf

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Probability

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
20 30 40 50

x

</div>
</div>
<div class="layoutArea">
<div class="column">
(*) Now use the central limit theorem to explain the results you observe.

</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
5 Exponential distribution

Let λ &gt; 0 be a positive real number. An exponential random variable X with rate parameter λ is a continuous random variable with density pλ : R → (0, ∞) defined by

􏰕0 if x &lt; 0 pλ(x) := λe−λx if x ≥ 0.

First prove that pλ is a well-defined probability density function.

Compute the population mean and variance of an exponential random variable X with parameter λ.

Compute the cumulative distribution function and the quantile function for exponential random variables with parameter λ.

Now implement a function called my_cdf_exp(). The function my_cdf_exp() should take as input two numbers x ∈ R and λ &gt; 0 and output the value of the cumulative distribution function FX (x) where X is an exponential random variable with rate parameter λ.

Check your function my_cdf_exp() gives rise to the following output:

## [1] 0.0000000 0.0000000 0.3934693 0.6321206 0.7768698 0.8646647

Type ?pexp into your R console to learn more about R’s inbuilt cumulative distribution function for the exponential

distribution. We can now confirm that our when λ = 1/2 as follows:

## [1] TRUE

Next implement a function called my_quantile_exp(). The function my_quantile_exp() should take as input

two arguments p ∈ [0,1] and λ &gt; 0 and output the value of the quantile function F−1(p) where X is an X

exponential random variable with rate parameter λ.

Once you have implemented your function compare with R’s inbuilt qexp function using the same procedure as we used above for the cumulative distribution function for inputs λ = 1/2 and p ∈ {0.01, 0.02, 0.03, . . . , 0.99}. Note that you don’t need to consider inputs p ≤ 0 or p ≥ 1 here.

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>lambda&lt;-1/2
map_dbl(.x=seq(-1,4),.f=~my_cdf_exp(x=.x,lambda=lambda))
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>test_inputs&lt;-seq(-1,10,0.1)
my_cdf_output&lt;-map_dbl(.x=test_inputs,.f=~my_cdf_exp(x=.x,lambda=lambda))
inbuilt_cdf_output&lt;-map_dbl(.x=test_inputs,.f=~pexp(q=.x,rate=lambda))
</pre>
<pre>all.equal(my_cdf_output,inbuilt_cdf_output)
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
6 Poisson distribution

Many discrete random variables have distributions supported on a finite set (eg. Bernoulli, Binomial). Poisson random variables are a family of discrete random variables with distributions supported on N0 := {0, 1, 2, 3, · · · }. Poisson random variables are frequently used to model the number of events which occur at a constant rate in situations where the occurance of individual events are independent. For example, we might use the Poisson distribution to model the number of mutations of a given strand of DNA per time unit, or the number of customers who arrive at store over the course of a day. Hence, like Binomial random variable, Poisson random variables can be used to model count data. The key difference is that Poisson random variables apply more readily to situations where there is no natural upper bound on the total count.

Take λ &gt; 0. The Poisson random variable X with parameter λ has probability mass function pλ : R → (0, ∞) defined by

</div>
</div>
<div class="layoutArea">
<div class="column">
􏰕λxe−λ for x ∈ N0

</div>
</div>
<div class="layoutArea">
<div class="column">
pλ(x) = x! 0

</div>
</div>
<div class="layoutArea">
<div class="column">
for x ∈/ N0. Show that pλ is a well-defined probability mass function. More precisely:

1. pλ(x)≥0forallx∈N0 2. 􏰖x∈R pλ(x) = 1.

Compute both the expectation and the variance of a Poisson random variable X with probability mass function pλ.

(**) Both Binomial and Poisson random variables can be used to model count data. Whilst Binomial random variables Z ∼ Binom(n,p) apply to situations where there is an upper bound n on the number of successes, Poisson random variables apply to situations where there is no natural upper bound on the total count. In fact the Poisson random variable X can be viewed as an approximation to Binomial random variable with very large n and np ≈ λ. This approximation is often used for computational reasons in situations where we want to model a Binomial random variable with a very large n and a small value of p.

As an optional extra, show the following: Suppose we fix λ ∈ R and a Poisson random variable X with expectaton λ, and take probabilities pn = nλ for each n ∈ N, and Binomial random variables Z ∼ Binom(n,pn). Then for each k ∈ N0 = {0,1,2,3,…} we have

n→∞ k! Youmaywanttousethefactthatforanyrealnumbert∈Rwehavelimn→∞􏰅1+nt􏰆n =et.

</div>
</div>
<div class="layoutArea">
<div class="column">
λk e−λ lim P(Zn =k)=P(X=λ)= .

</div>
</div>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column">
7 (**) The law of large numbers and Hoeffding’s inequality

Prove the following version of the weak law of large numbers.

Theorem (A law of large numbers). Let X : Ω → R be a random variable with a well-defined expectation μ := E(X) and variance σ2 := Var(X). Let X1,…,Xn : Ω → R be a sequence of independent copies of X.

</div>
</div>
<div class="layoutArea">
<div class="column">
Then for all ε &gt; 0,

</div>
</div>
<div class="layoutArea">
<div class="column">
􏰚􏰌􏰌1􏰁n 􏰌􏰌􏰛 limP 􏰌􏰌 Xi−μ􏰌􏰌≥ε =0.

􏰌

Now investigate Hoeffding’s for sample averages of bounded random variables. How does this compare to the law of large numbers?

</div>
</div>
<div class="layoutArea">
<div class="column">
n→∞ 􏰌n i=1

You may want to begin by looking up Chebyshev’s inequality.

</div>
</div>
<div class="layoutArea">
<div class="column">
9

</div>
</div>
</div>
