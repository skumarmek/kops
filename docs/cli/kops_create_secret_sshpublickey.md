## kops create secret sshpublickey

Create a ssh public key.

### Synopsis


Create a new ssh public key, and store the key in the state store.  The key is not updated by this command.

```
kops create secret sshpublickey
```

### Examples

```
  # Create an new ssh public key called admin.
  kops create secret sshpublickey admin -i ~/.ssh/id_rsa.pub \
  --name k8s-cluster.example.com --state s3://example.com
```

### Options

```
  -i, --pubkey string   Path to SSH public key
```

### Options inherited from parent commands

```
      --alsologtostderr                  log to standard error as well as files
      --config string                    config file (default is $HOME/.kops.yaml)
      --log_backtrace_at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log_dir string                   If non-empty, write log files in this directory
      --logtostderr                      log to standard error instead of files (default false)
      --name string                      Name of cluster
      --state string                     Location of state storage
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          log level for V logs
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO
* [kops create secret](kops_create_secret.md)	 - Create a secret.

