# Running tests

## Steps

* install oc client at ~/oc_client/oc
* create python3 venv, clone patterns repository
* export KUBECONFIG=\<path to hub kubeconfig file>
* export KUBECONFIG_EDGE=\<path to edge kubeconfig file>
* export INFRA_PROVIDER=\<infra platform description>
* (optional) export WORKSPACE=\<dir to save test results to> (defaults to /tmp)
* cd \<pattern dir>/tests/interop
* pip install -r requirements.txt
* ./run_tests.sh

## Results

* results .xml files will be placed at $WORKSPACE
* test logs will be placed at $WORKSPACE/.results/test_execution_logs/
* CI badge file will be placed at $WORKSPACE
