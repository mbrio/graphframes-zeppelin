# GraphFrame on Zeppelin

There's a bit of a trick to getting the graphframes library to work on
zeppelin. This repository has a package setup that can be deployed with
minimal effort. This package is for the following configuration:

* EMR - 5.7.0
* Spark - 2.1.1
* Zeppelin - 0.7.2
* Hadoop - 2.7.3
* GraphFrames - 0.5.0

1. Upload `graphframes-lib.tar.gz` to the `hadoop` user directory on EMR:

```
$ scp graphframes-lib.tar.gz hadoop@ec2-##-###-###-##.compute-1.amazonaws.com:~/
```

2. SSH into the EMR cluster

```
$ ssh hadoop@ec2-##-###-###-##.compute-1.amazonaws.com
```

3. Uncompress the `graphframes-lib.tar.gz` file:

```
$ tar xzvf graphframes-lib.tar.gz
```
