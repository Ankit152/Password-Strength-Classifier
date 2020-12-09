# Password Strength Classifier

<div>
    A Machine Learning model that predicts whether the password is strong or not.
</div>

<p>The passwords used in our analysis are from 000webhost leak that is available online. How did we figure out which passwords were stronger and which were weaker? Well, there is a tool called PARS by Georgia Tech university which have all the commercial password meters integrated into it. All I did was give that tool all the passwords and it gave me new files for each commercial password strength meter. The files contained the passwords with one more column i.e their strength based on the commercial password strength meters.</p>

<p>The commercial password strength algorithms I used are of Twitter, Microsoft and battle. How is this algorithm different from these strength meters? First of all, it is entirely based on machine learning rather than on rules. Secondly, I only kept those passwords that were flagged weak, medium and strong by all three strength meters. This means that all the passwords were indeed either weak, medium or strong.</p>

<p>I had a total of 3 million passwords but after taking the intersection of all classifications of commercial meters, I was left with 0.7 million passwords. The reduction was because of the fact that I only used passwords that were flagged in a particular category by all three algorithms.</p>

