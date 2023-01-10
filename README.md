## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add gripo-operators https://gripo-io.github.io/operator-charts/

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the strimzi operator chart:

    helm install strimzi-operator gripo-operators/sample-kafka

To uninstall the chart:

    helm delete strimzi-operator
