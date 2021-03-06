# ⚓️ Open Innovation Labs Helm Charts

![Release Charts]

A collection of Helm Charts to support [Labs Developer Experience](https://github.com/kborup-redhat/ubiquitous-journey)

## 🧰 Add this Helm Repo to your local 🧰
```
helm repo add rht-labs https://kborup-redhat.github.io/helm-charts
```

## 🏃‍♀️💨 How do I run a chart?
Login to your cluster and into your destination project. To install any given Chart using the default values just run:
```bash
helm install $NAME kborup-redhat/$CHART_NAME
eg:
helm install my-jenkins kborup-redhat/jenkins
```
Where:
* $NAME - is the name you want to give the installed Helm App
* $CHART_NAME - name of the chart found in `charts` directory


## 🏃‍♂️💨Customisation to a chart prior to install
For each chart, navigate to the root of it for the readme and default values. To over ride them, you could create your own `my-values.yaml` and make your changes there before installing
```bash
helm install $NAME -f my-values.yaml kborup-redhat/$CHART_NAME
eg:
helm install my-jenkins -f my-values.yaml kborup-redhat/jenkins
```

## 👩‍🏫 Chart README Files
For more info on each chart checkout these!
* [jenkins](/charts/jenkins)
* [sonarqube](/charts/sonarqube)
* [bootstrap-project](/charts/bootstrap-project)
* [operatorhub](/charts/operatorhub)
* [pact-broker](/charts/pact-broker)
