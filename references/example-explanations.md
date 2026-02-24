# Example Explanations

These examples demonstrate the style, depth, and structure expected from visual-rabbit-hole explanations.

## Example 1: Explaining "Recursion"

**User**: Explain recursion to me

**Response**:

### The Analogy: Russian Nesting Dolls

Imagine you have a Russian nesting doll (matryoshka). To find the smallest doll, you:
1. Open the current doll
2. If there's a doll inside, repeat from step 1
3. If there's no doll inside — you found the smallest one. Done!

That's recursion: **a process that calls itself with a smaller version of the same problem until it hits a stopping point (the base case).**

### The Diagram

```
findSmallest(🪆🪆🪆🪆)
  │
  ├─ "Is there a doll inside?" → Yes
  │   └─ findSmallest(🪆🪆🪆)
  │       │
  │       ├─ "Is there a doll inside?" → Yes
  │       │   └─ findSmallest(🪆🪆)
  │       │       │
  │       │       ├─ "Is there a doll inside?" → Yes
  │       │       │   └─ findSmallest(🪆)
  │       │       │       │
  │       │       │       └─ "Is there a doll inside?" → No!
  │       │       │           BASE CASE → return 🪆
  │       │       │
  │       │       └─ returns 🪆
  │       └─ returns 🪆
  └─ returns 🪆
```

### The Gotcha

The #1 mistake: **forgetting the base case**. Without a stopping condition, your nesting dolls go on forever — in code, that's a stack overflow.

### Go Deeper (The Rabbit Hole)

- **Tail recursion** — Why some languages optimize recursive calls to run as fast as loops
- **The call stack** — What physically happens in memory when functions call themselves
- **Divide and conquer** — The algorithm family that makes recursion powerful (mergesort, quicksort)
- **Memoization** — How to avoid re-solving the same sub-problems (leads into dynamic programming)

---

## Example 2: Explaining "Inflation" (non-technical)

**User**: What is inflation and why does it happen?

**Response**:

### The Analogy: Musical Chairs with Money

Imagine 10 people at an auction with $100 each, bidding on 10 pizzas. Pizzas sell for ~$100.

Now give everyone $200 instead. Same 10 pizzas, but double the money chasing them. Pizzas sell for ~$200. **Nothing real changed — there's no more pizza — but the price doubled because there's more money competing for the same stuff.**

That's inflation at its core: **too much money chasing too few goods.**

### The Diagram

```
NORMAL STATE                    INFLATION
┌─────────────────┐            ┌─────────────────┐
│  💰💰💰          │            │  💰💰💰💰💰💰    │
│  Money supply    │            │  More money!     │
│                  │            │                  │
│  🍕🍕🍕          │            │  🍕🍕🍕          │
│  Same goods      │            │  Same goods      │
│                  │            │                  │
│  Price: $10/🍕   │            │  Price: $20/🍕   │
└─────────────────┘            └─────────────────┘

        The Three Main Causes:

  Demand-Pull          Cost-Push          Money Supply
  ──────────          ──────────         ────────────
  People want         It costs more      Government
  more stuff    →     to make stuff  →   prints more
  than exists         (oil, wages)       money

  "Too many           "Costs go up,      "More dollars
   dollars             prices             chasing same
   chasing             follow"            goods"
   too few goods"
```

### The Gotcha

People think inflation is always bad. Moderate inflation (~2%) is actually considered healthy — it encourages spending and investment. **Deflation** (falling prices) is often worse: people delay purchases ("it'll be cheaper tomorrow"), businesses earn less, lay off workers, spiral downward.

### Go Deeper (The Rabbit Hole)

- **The Phillips Curve** — The debated tradeoff between inflation and unemployment
- **Hyperinflation** — What happens when inflation spirals out of control (Weimar Germany, Zimbabwe)
- **Central bank interest rates** — The main tool used to fight inflation, and why raising rates works
- **Real vs nominal values** — How to think about money's actual purchasing power over time

---

## Example 3: Using Web Search

**User**: Explain how mRNA vaccines work

(In this case, use WebSearch to find a recent, clear source to ground the explanation with accurate, current details. Then structure the response the same way — analogy, diagram, gotcha, rabbit hole.)
