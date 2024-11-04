# hazeltest-charts

Contains Helm charts for [Hazeltest](https://github.com/AntsInMyEy3sJohnson/hazeltest).

## How To Work With This Repository
Branch [`gh-pages`](https://github.com/AntsInMyEy3sJohnson/hazeltest-charts/tree/gh-pages) represents a non-OCI
Helm repository, offering various Helm charts plus an `index.yaml` file so your Helm CLI can find, list, and query them.

Here's how you can use this repository using your Helm CLI:

### Step 1: Add Repository

```bash
helm repo add hazeltest https://raw.githubusercontent.com/antsinmyey3sjohnson/hazeltest-charts/gh-pages
```

### Step 2: Update Repository List

```bash
helm repo update
```

### Step 3: Find Chart You Wish To Install

If you would like to see and install only the most recent chart version:
```bash
helm search repo hazeltest
```

Sample output:
```bash
NAME               	CHART VERSION	APP VERSION	DESCRIPTION
hazeltest/hazeltest	1.3.0        	0.16.0     	A Helm chart for deploying Hazeltest on Kubernetes
```

Or, in case you would like to review the complete list of chart versions available in this repository, and then pick one from the list:
```bash
helm search repo hazeltest --versions
```

Which would then give you something like the following:

```bash
NAME               	CHART VERSION	APP VERSION	DESCRIPTION
hazeltest/hazeltest	1.3.0        	0.16.0     	A Helm chart for deploying Hazeltest on Kubernetes
hazeltest/hazeltest	1.2.1        	0.10.1     	A Helm chart for deploying Hazeltest on Kubernetes
hazeltest/hazeltest	1.2.0        	0.8.0      	A Helm chart for deploying Hazeltest on Kubernetes
hazeltest/hazeltest	1.1.1        	0.5.2      	A Helm chart for deploying Hazeltest on Kubernetes
hazeltest/hazeltest	1.1.0        	0.5.2      	A Helm chart for deploying Hazeltest on Kubernetes
```

### Step 4: Install Desired Chart

```bash
helm upgrade --install <release-name> hazeltest/hazeltest -n <namespace> --version <version>
```

### Step 5 (Optional): Reward Yourself With Cookie
Wohooo, you did it! Marvellous job. Go reward yourself with a cookie!*

(* Not sponsored by cookie lobby.)

⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣴⣶⣿⣿⡿⠿⠷⣶⣤⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⢀⣴⣾⣿⣿⣿⣿⣿⣿⣇⠀⠀⢸⣿⣿⣿⣦⡀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⢀⣴⣿⡿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣦⡀⠀⠀⠀⠀
⠀⠀⠀⢠⣿⡟⠁⠀⠀⢹⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⡀⠀⠀⠀
⠀⠀⢠⣿⣿⣿⣦⣄⣠⣼⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⢿⣿⣿⣿⣷⠀⠀⠀
⠀⠀⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡏⠀⠀⢹⣿⣿⣿⡇⠀⠀
⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣶⣶⣿⣿⣿⣿⣿⠀⠀
⠀⠀⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠀⠀
⠀⠀⠈⢿⣿⣿⣿⣿⠟⠻⣿⣿⠋⠀⠉⣿⣿⣿⣿⣿⣿⣿⣿⡏⠀⢙⣿⠃⠀⠀
⠀⠀⠀⠈⢿⣿⣿⠁⠀⠀⠘⣿⣆⠀⢀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠏⠀⠀⠀
⠀⠀⠀⠀⠀⠙⢿⣦⣤⣤⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠋⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠙⠿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠉⢹⣿⣿⡿⠟⠁⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠛⠿⠿⣿⣿⣿⣷⡤⠾⠛⠉⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀








