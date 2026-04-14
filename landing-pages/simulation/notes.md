# Simulation page

https://simulation.govstack.global/

![mainPage](images/main-page.png)

Simulation and  [Unconditional social cash transfer](../../use-cases/usct/notes.md) uses the same [frontend repository](https://github.com/GovStackWorkingGroup/sandbox-usecase-usct-frontend).

## Useful commands


```shell
helm install simulation ./landing-pages/simulation  --create-namespace --namespace simulation
```

```shell
helm upgrade --install simulation ./landing-pages/simulation --create-namespace --namespace simulation

```