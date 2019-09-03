## kyma test run

Runs tests on a Kyma cluster

### Synopsis

Runs tests on a Kyma cluster

If you don't provide any specific test definitions, all available test definitions will be added to the newly created test suite.
If you don't specify the value for the -n flag, the name of the test suite name will be autogenerated.

To execute all test defintions, run the"example-test" test suite:
kyma test run -n example-test


```
kyma test run <test-definition-1> <test-defintion-2> ... <test-definition-N> [flags]
```

### Options

```
      --concurrency int   Number of tests to be executed in parallel. (default 1)
  -c, --count int         Number of execution rounds for each test in the suite. You cannot configure this value in parallel with max-retries (default 1)
  -h, --help              help for run
      --max-retries int   Number of retries for a failed test. (default 1)
  -n, --name string       Name of the new test suite
```

### Options inherited from parent commands

```
      --kubeconfig string   Path to kubeconfig (default "/Users/i504462/.kube/config")
      --non-interactive     Do not use spinners
  -v, --verbose             verbose output
```

### SEE ALSO

* [kyma test](kyma_test.md)	 - Run tests on a provisioned Kyma cluster

###### Auto generated by spf13/cobra on 3-Sep-2019