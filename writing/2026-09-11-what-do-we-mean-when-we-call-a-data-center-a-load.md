# What Do We Mean When We Call a Data Center a Load?

*September 11, 2026*

None of the ideas in this note are particularly new. What is new, at least to me, is how differently I started thinking about electricity demand after trying to model it.

I used to think the most interesting question about AI data centers and electricity was mostly about scale.

They use a lot of power. They are growing quickly. Utilities have to build around them. The natural questions seem quantitative: how many gigawatts, how fast, and where?

But while working on related research, I kept running into something that made the usual picture feel incomplete. A data center may appear in an electricity model as a load, but the thing behind that load is computation. And computation has its own structure.

Some work has to happen now. Some can happen later. Some is valuable enough that interruption is extremely costly. Other work may be movable in time or across machines. The same amount of electricity consumption can therefore represent very different obligations.

That sounds like a technical detail. I initially treated it as one.

I am starting to think it is closer to the main question.

The word *load* is useful because it compresses a complicated object into a number the power system can work with. But compression hides things. Two facilities that consume the same number of megawatt-hours may respond very differently to scarcity, prices, reliability incentives, or constraints on the grid. Looking only at total consumption can make those differences disappear.

This has changed the way I think about the usual supply-and-demand picture of electricity markets. We often draw demand as the passive side of the system: electricity is needed, and generators, networks, and markets figure out how to serve it.

Large computational loads make that story less clean.

A data center is certainly a customer. But depending on how its computing needs are organized, it may also have choices about when electricity is most valuable, what kind of reliability it is willing to pay for, and how much its demand can respond to conditions on the system.

None of this means that data centers are unique. Industrial loads have been flexible for a long time, and demand response is hardly a new idea. What I find interesting is that AI infrastructure brings these questions back at an unusual scale and with a new object sitting behind electricity demand: computation.

That makes me more cautious about statements like “AI will require X amount of electricity.” The number matters. But it does not tell us everything we would want to know about the interaction between AI infrastructure and the grid.

The harder questions are about the shape of that demand: when it appears, how rigid it is, how reliability is valued, and how those characteristics interact with the rules and incentives of electricity markets.

Working on this topic has made me realize that modeling choices sometimes reveal conceptual choices. Deciding how to represent a data center is not just a mathematical convenience. It forces you to decide what you think the economic object actually is.

I do not have a clean answer yet.

But I now find myself less interested in asking only:

**How much electricity will AI consume?**

and more interested in asking:

**What do we mean when we call an AI data center a load?**
