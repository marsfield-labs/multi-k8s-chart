# Chart `multi-k8s`

This project builds a chart based on previous `multi-k8s` project. It aims to build a chart that can be deployed easily in different kubernetes environments.

## Build basic chart files

Run following command to create initial files:

```sh
helm create multi-k8s
```

This will create a folder called `multi-k8s`, we can check its contents.

```txt
cd multi-k8s
$ ls 
charts/  .git/  templates/  Chart.yaml  .helmignore  README.md  values.yaml
```

For explanation of chart folder structure, check out [this page](https://helm.sh/docs/topics/charts/#the-chart-file-structure).

## Package chart

We can build our chart package now, run:

```sh
helm package multi-k8s
```

This will create a package archive in current directory, e.g. `multi-k8s-0.1.0.tgz`.

## References

* [Chart doc](https://helm.sh/docs/topics/charts/)
