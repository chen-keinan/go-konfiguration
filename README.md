[![Go Report Card](https://goreportcard.com/badge/github.com/chen-keinan/beacon)](https://goreportcard.com/report/github.com/chen-keinan/beacon)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/chen-keinan/beacon/blob/main/LICENSE)
[![Build Status](https://travis-ci.com/chen-keinan/kube-beacon.svg?branch=main)](https://travis-ci.com/chen-keinan/kube-beacon)
[![Coverage Status](https://coveralls.io/repos/github/chen-keinan/kube-beacon/badge.svg?branch=main)](https://coveralls.io/github/chen-keinan/kube-beacon?branch=main)
[![Gitter](https://badges.gitter.im/kube-beacon/community.svg)](https://gitter.im/kube-beacon/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
# go-simple-config
> Go Simple config is an open source configuration lib for storing and accessing configuration data with minimal dependencies
>

### supported configuration files:

- yaml
- json
- properties
- Environment variable

### usage example
```
func readConfig() error{
    c := New()
    err := c.Load("config.json")
    
    if err != nil {
       return err
     }	 
     
    fmt.Print(c.GetValueString("SERVER.host"))
}
```