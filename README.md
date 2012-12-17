welcome to hft!
===============

HFT is a small project with a big ambition. We aim to build the worlds fastest algorithmic trading platform using the best off-the-shelf open source technology stack we can find.

Even better, we are aiming for an overall design that is minimal, simple and robust.  Ultimately, we would like the high-frequency community, whether serious professional or keen amateur enthusiast to look towards hft as the backbone of their next project.

There's not much to see here right now, but check back soon and see how we're doing.

## incoming ##
1. algorithms: I'm trying to get some discussion and collaboration
   going with respect to an algorithm classification scheme. I would like to code up some algorithmic approaches that:
  - are security detail agnostic (ie can be applied to any tradable asset)
  - are divided into three categories: functions of historical price
    (technicals), functions of the historical prices of other
    securities (stat arb) and functions of factors exogenous to price
    (fundamentals).
  
2. prototype: I like your idea of reusable components but I think the
   group would need a working prototype. I'm new to high-frequency
   trading and I personally need to build and run a complete system to
   develop intuition. I suspect there are many others in the same boat.


## component radar ##

Let us know if a trading solution or component should be on our R&D radar:

- http://tradexoft.wordpress.com
- http://esper.codehaus.org
- http://code.google.com/p/tradelink/



### lockfree++ ###

A low-latency messaging system impleneting the Actor model.

http://tradexoft.com



# algorithm design #

This is a summary of discussions on algorithm classification that will eventually become a coding specification for the algorithm component of `hft`

The lists below are examples of categories and not meant to be exhaustive.

## data-set choice ##

### Price Endogenous ###

Algorithms that are endogenous to price

- moment-based calculations
  - moving average
  - GARCH
  - volatility
  - momentum
- technical analytics

### Market Structure Endogenous ###

Algorithms that are endogenous to Price and market components closely related to a single security such as:
- volume
- bid/ask
- market depth, order book

### Statistical Arbitrage ###

Algorithms that look to exploit near-arbitrage bound relationships between securities. 
- VIX versus SP500 versus options
- cross-correlation or lead-lag relationships between securities


### Exogenous ###

Algorthims that seek to exploit relationships between price and factors external to the security market price information set.

- fundamentals
- twitter mentions
- earnings announcement/ event-based analytics

## time horizon choice ##


## algorithmic theoretica choice ##

- linear 
  - regression
- non-linear
  - NN
  - GA
- parameter fit 
  - local versus global minima
  - stationary versus non-stationary (versus semi-stationary)
- contrarian versus continuation (???)  

## trading choices ##

- leverage employed
- transactional cost importance
- entry and exit methodologies
- security selection
- P&L distribution choices (objective function)


# linkedin discussion groups #

http://www.linkedin.com/groups?home=&gid=62719&trk=anet_ug_hm

