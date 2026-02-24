# Example Explanations

These examples demonstrate the style, depth, and structure expected from visual-rabbit-hole explanations.

## Example 1: Explaining "Recursion"

**User**: Explain recursion to me

**Response**:

### The Setup

Here's a problem: you have a pile of nested boxes, and somewhere in the smallest box is a key. You don't know how deep it goes. How do you find it?

You could try to plan ahead — but you don't know the depth. So what if you just said: "open the box. If there's another box inside, do the same thing. If there's a key, stop."

That's it. That's recursion. **You just described a process that uses itself as its own instruction manual.**

### The Analogy: Russian Nesting Dolls

Think of a matryoshka doll. To find the smallest one:
1. Open the current doll
2. If there's a doll inside, repeat from step 1
3. If there's no doll inside — you found it. Done.

The beautiful part? You didn't need different instructions for each layer. **One rule handled all of them.**

### The Diagram — Watch it unfold and fold back

```
UNFOLDING (going deeper)              FOLDING BACK (returning)

findSmallest(🪆🪆🪆🪆)                 findSmallest(🪆🪆🪆🪆)
  │                                      ▲
  ▼ open it                              │ returns 🪆
findSmallest(🪆🪆🪆)                   findSmallest(🪆🪆🪆)
  │                                      ▲
  ▼ open it                              │ returns 🪆
findSmallest(🪆🪆)                     findSmallest(🪆🪆)
  │                                      ▲
  ▼ open it                              │ returns 🪆
findSmallest(🪆)                       findSmallest(🪆)
  │                                      │
  └─ nothing inside!                     └─ BASE CASE: return 🪆
     STOP HERE ─────────────────────────────►
```

Notice: it goes all the way down first, *then* all the way back up. Two phases, one rule.

### The Gotcha

The #1 mistake: **forgetting the base case**. Without "if there's no doll inside, stop" — your process never ends. In code, that's a stack overflow. Every recursive function needs its "smallest doll."

### The Rabbit Hole

**Go Deeper:**
- **The call stack** — What physically happens in memory during those two phases (unfold/fold back)
- **Tail recursion** — A trick where the "fold back" phase disappears entirely, making recursion as fast as a loop
- **Divide and conquer** — Split the problem, solve each half the same way. This is how mergesort and quicksort work — and why they're so elegant.

**Surprising Connections:**
- **Fractals in nature** — Romanesco broccoli, coastlines, blood vessels — nature uses the same trick: one rule applied at every scale. Recursion isn't just a coding pattern, it's a structure the universe keeps reusing.
- **Infinite regress in philosophy** — "Who created the creator?" is a recursion without a base case. Philosophers have debated this for millennia — turns out it's the same bug programmers hit.

---

## Example 2: Explaining "Inflation" (non-technical)

**User**: What is inflation and why does it happen?

**Response**:

### The Setup

Here's something weird: a cup of coffee cost $0.25 in 1970. Now it's $5. The coffee didn't get 20x better. So what happened to the money?

### The Analogy: An Auction with Too Much Cash

Imagine 10 people at an auction, each with $100, bidding on 10 pizzas. Pizzas sell for ~$100.

Now the auctioneer hands everyone an extra $100. Same 10 pizzas. But now everyone's waving $200 around. What happens?

Pizzas sell for ~$200. **Nothing real changed — no extra pizza was created — but every dollar became worth less because there are more of them competing for the same stuff.**

### The Diagram — Before and After

```
BEFORE                              AFTER
┌─────────────────┐                ┌─────────────────┐
│  💰💰💰          │                │  💰💰💰💰💰💰    │
│  Money supply    │                │  More money!     │
│                  │       ──►      │                  │
│  🍕🍕🍕          │                │  🍕🍕🍕          │
│  Same goods      │                │  Same goods      │
│                  │                │                  │
│  Price: $10/🍕   │                │  Price: $20/🍕   │
└─────────────────┘                └─────────────────┘

But wait — where does the extra money come from?

  Demand-Pull          Cost-Push          Money Printing
  ──────────          ──────────         ──────────────
  People suddenly     It costs more      Central bank
  want more stuff     to make stuff      creates more
  than exists         (oil, wages)       currency

  "Everyone wants     "Costs go up,      "More dollars,
   the same pizza"     pizza follows"     same pizza"
```

### The Gotcha

You'd think inflation is always bad. But here's the twist: moderate inflation (~2%) is considered *healthy*. It nudges people to spend and invest instead of hoarding cash. **Deflation** — falling prices — sounds great until you realize everyone stops buying ("it'll be cheaper tomorrow"), businesses earn less, lay off workers, and the economy spirals. The real enemy isn't rising prices — it's *unpredictable* prices.

### The Rabbit Hole

**Go Deeper:**
- **Central bank interest rates** — The main lever used to fight inflation, and the elegant logic behind why raising rates cools things down
- **Hyperinflation** — What happens when inflation breaks loose entirely (Zimbabwe printed $100 trillion bills)
- **Real vs nominal values** — How to stop being fooled by big numbers and think about what money can actually *buy*

**Surprising Connections:**
- **Equilibrium in chemistry** — Le Chatelier's principle says: disturb a system at equilibrium and it pushes back to restore balance. Central banks do the exact same thing. Economics and chemistry are both studying systems that self-correct — with the same math.
- **Tragedy of the commons in ecology** — Everyone acting rationally (spending more before prices rise) makes the collective outcome worse (prices rise faster). Same structure as overfishing, climate change, and antibiotic resistance.

---

## Example 3: Using Web Search

**User**: Explain how mRNA vaccines work

(In this case, use WebSearch to find a recent, clear source to ground the explanation with accurate, current details. Then structure the response the same way — setup, analogy, diagram, gotcha, rabbit hole.)
