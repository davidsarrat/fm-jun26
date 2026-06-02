## The whole API is one recipe

<div class="grid grid-cols-2 gap-6 mt-3 items-center">
<div>

```r
flower <- ds.flower.connect(conns)

recipe <- ds.flower.recipe(
  model         = ds.flower.model.sklearn_logreg(),
  strategy      = ds.flower.strategy.fedavg(),
  target_column = "diagnosis",
  num_rounds    = 10L
)

result <- ds.flower.run(flower, recipe)
```

</div>
<div>

A recipe is just **four plain-language choices**:

- `model` &mdash; **what** to train
- `strategy` &mdash; **how** to combine sites
- `target_column` &mdash; the **outcome**
- `num_rounds` &mdash; **how long**

<div class="mt-3" v-click>

Connect, compose, run. **Privacy is enforced by the server**, so it holds no matter what the analyst writes.

</div>

</div>
</div>
