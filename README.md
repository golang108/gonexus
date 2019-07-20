# gonexus

Provides a go client library for connecting to, and interacting with, [Sonatype](//www.sonatype.com) Nexus applications such as Nexus Repository Manager and Nexus IQ Server.

## Organization of this library
The library is broken into two packages. One for each application.

### nexusrm [![GoDoc](http://godoc.org/github.com/sonatype-nexus-community/gonexus/rm?status.png)](http://godoc.org/github.com/sonatype-nexus-community/gonexus/rm) [![nexusrm coverage](https://gocover.io/_badge/github.com/sonatype-nexus-community/gonexus/rm?0 "nexusrm coverage")](http://gocover.io/github.com/sonatype-nexus-community/gonexus/rm)

Create a connection to an instance of Nexus Repository Manager
```go
import "github.com/sonatype-nexus-community/gonexus/rm"

rm, err := nexusrm.New("http://localhost:8081", "username", "password")
if err != nil {
    panic(err)
}
```

### nexusiq [![GoDoc](http://godoc.org/github.com/sonatype-nexus-community/gonexus/iq?status.png)](http://godoc.org/github.com/sonatype-nexus-community/gonexus/iq) [![nexusiq coverage](https://gocover.io/_badge/github.com/sonatype-nexus-community/gonexus/iq?0 "nexusiq coverage")](http://gocover.io/github.com/sonatype-nexus-community/gonexus/iq)

Create a connection to an instance of Nexus IQ Server
```go
import "github.com/sonatype-nexus-community/gonexus/iq"

iq, err := nexusiq.New("http://localhost:8070", "username", "password")
if err != nil {
    panic(err)
}
```

## The Fine Print
It is worth noting that this is **NOT SUPPORTED** by [Sonatype](//www.sonatype.com), and is a contribution of HokieGeek
plus us to the open source community (read: you!)

Remember:

* Use this contribution at the risk tolerance that you have
* Do **NOT** file Sonatype support tickets related to this
* **DO** file issues here on GitHub, so that the community can pitch in
