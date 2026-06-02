> I should have mentioned that some pictures and a lot of info is just from blanchard. Bless that book. I'll take it off the internet if they find it problematic. 
- Money is something that you can use for transactions that pays no interest. It has two types - currency and deposit accounts
- Bonds are financial instruments that pay a positive interest rate, they are used to control the supply of money
- Clearly, the higher the interest rate, the more reason there is to hold them. Higher interest rates cause an individual's wealth in money to reduce and in bonds to increase
## Money Demand
- We can write the demand for money in terms of a function of the interest rate(L(i)), nominal income (Y):
- $$M^d = YL(i)$$
- The higher the interest rate, the lower the money demand. This means the demand curve for money is downward sloping against interest rate. 
- ![[Pasted image 20260204222557.png]]
## LM Relation
- Suppose theres a central bank that has the job to control the financial market. If it chooses to supply an amount of money $M^S$
- For equilibrium in financial markets, the money supplied must be equal to the money demanded. 
- $$M^S = YL(i)$$
- The interest rate must be such that people (all combined) hold an amount of money equal to how much is supplied
- I read at the end of the chapter, however, that the money supplied determines the interest rate, not the other way around. 
## Monetary Policy
- The way central banks change the supply of money is through buying and selling of bonds
- If they want to increase the amount of money in circulation, they create it out of thin air and buy bonds with it (Who puts these bonds up? how do they know what interest rate to put it at???). This is called an expansionary open market operation
- They sell bonds in a contractionary open market operation
- I really want to explain how bonds work, but as a prank, I'll leave calculating bond yields to the reader. Haha
### Liquidity Trap
- You cannot have interest rates below zero.
- This bears an interesting consequence on the demand of money
- Once you have interest rate of zero set by a central bank, the consumer is indifferent to how much money they want to hold (after the minimum required for transactions)
- Since the central bank doesn't control the minds of every human and tell them what the interest rate is (instead decides the interest rates by buying and selling bonds), if they want to cause a greater supply of money in the economy, they can't. Since increasing the money supply doesn't change the interest rate. 
- The above is a liquidity trap. People are willing to hold more liquidity at the same interest rate.
- This is apparently important for a central bank to consider when they want to increase the money supply to increase output and boost spending when the economy is stuck in a liquidity trap. 
> I think I need a case study to make any sense of this

## LM relation, but better
- So in real life, all the money someone has isn't kept in currency. It's divided into deposit accounts and currency. 
- Banks keep reserves of  some of the funds they receive and the rest they invest in loans and other forms of wealth such as bonds
- There is something such as a reserve ratio that banks in modern economies are mandated to maintain. This is the ratio of the reserve to the liability of the bank (the full amount of all deposits at that given time
- Cool visual I have ripped out of Blanchard ![[Pasted image 20260204233315.png]]
- $CU^d$ represents currency demand. So not all money is money demanded from central banks. We only demand the reserves of banks and currency demanded by people. Keeping that in mind, we can write an equation, like above: $$(currency\space demanded+reserves\space demanded) = Money\space supplied$$
- $$(cM^d+\theta(1-c)M^d) = M^s$$
- or the beautiful way, it's written in the visual, with H as the money supplied
- Also, btw, $\theta$ is the reserve ratio in the equation above
- Since $M^d = YL(i)$, we can write the above nicely
- $$(c+\theta(1-c))YL(i) = M^s$$
- or $$M^s\frac{1}{1+\theta(1-c)} = YL(i)$$
- so the money demanded equals the money supplied. Which is the actual money the reserve bank needs to create out of thin air multiplied by the money multiplier
- So the actual meaning of the money multiplier goes something like:(assuming c=0) so the central bank buys 100 rupees worth of bonds in the market to increase the money supplied. This causes the person who they bought those bonds doesn't want to hold any money (c=0)in currency, so they put all of it in their deposit account, which causes the bank to buy bonds (not really, but lets suppose loans are just bonds) with $(1-\theta)$ amount of the 100 rupees. This goes on and on with each seller of bonds depositing money, and having the same ratio of it used for bonds until that money is all either invested in bonds or kept in the reserve of the bank strictly adhering to the reserve ratio. This can be expressed as a geometric series, which simplifies to the above equation