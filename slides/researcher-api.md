## The whole API is one recipe

<div class="grid grid-cols-2 gap-6 mt-3 items-center">
<div>

```r
# DataSHIELD login loads each site's table into D
conns  <- datashield.login(
  logins, assign = TRUE, symbol = "D"
)

flower <- ds.flower.connect(conns, symbol = "D")

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

The data is the table DataSHIELD already loaded into `D`. The recipe is just **four plain-language choices**:

- `model`: **what** to train
- `strategy`: **how** to combine sites
- `target_column`: the **outcome**
- `num_rounds`: **how long**

<div class="mt-3" v-click>

Load, connect, compose, run. **Privacy is enforced by the server**, so it holds no matter what the analyst writes.

</div>

</div>
</div>
