Learning in Public Series #11

What Vibe Coding Is Actually Good At

It’s hard to believe it’s only been about ten months since Karpathy coined the term “vibe coding.” In the age of AI, time feels compressed.

I’ve tried vibe coding, enjoyed its benefits, and also learned—sometimes the hard way—where it breaks down.

Vibe coding works best as an alignment accelerator. PRDs, design docs, and Figma are all useful, but each has limitations. Written specs get interpreted differently. Static designs miss flows. Early discussions can stretch on before people are actually aligned.

Starting with a vibe-coded prototype changes that dynamic. Whether led by an engineer or a designer, a working artifact gives everyone something concrete to react to. Conversations become sharper, decisions get made faster, and alignment that might have taken weeks can happen in days.

The code that comes out of early vibe coding usually isn’t something you’d want to ship. But it’s often a solid reference implementation. Current models can produce something ~70–80% there visually and functionally—enough to explore ideas, demo to customers, and align stakeholders. I’ve even heard of teams reverse-engineering prototypes back into PRDs to drive alignment in larger organizations.

The key is knowing when to switch gears. Vibe mode is not engineering mode. At some point, you have to slow down, revisit the design, think through proper data modeling, and make explicit tradeoffs. Skipping that transition is where problems start.

I’ve had failures here too. In one hackathon, under time pressure, I let AI generate a ton of code without slowing down to fully follow through on each step. When I tried to get into the code to fix things, it became unbearable due to the sheer amount of suboptimal, AI-generated code. Prompting forward felt like the only way out.

That experience clarified the boundary for me. Since then, I follow a lightweight design process, using AI as a thought partner, scoping each generation to a small outcome and reviewing it rather than letting it run unchecked. Vibe coding still shines for early exploration, cross-functional alignment, and demos—but only when paired with this oversight.