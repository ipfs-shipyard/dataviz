# IPFS Data Visualizations

[![](https://img.shields.io/badge/made%20by-Protocol%20Labs-blue.svg?style=flat-square)](http://ipn.io)
[![](https://img.shields.io/badge/project-IPFS-blue.svg?style=flat-square)](http://ipfs.io/)
[![](https://img.shields.io/badge/freejs-%23ipfs-blue.svg?style=flat-square)](http://webchat.freenode.net/?channels=%23ipfs)

![](https://cdn.rawgit.com/jbenet/contribute-ipfs-gif/master/img/contribute.gif)

[![Stories in Ready](https://badge.waffle.io/ipfs/dataviz.svg?label=ready&title=Ready)](http://waffle.io/ipfs/dataviz)


## graphmd

** Status: stable **

Graphs of Merkel DAGs from the command line.

![](https://ipfs.io/ipfs/QmbefthRKDReojALJi8nGPwvUVPqe1aXdoD9ysX44aUfvG/graph.png)

More information here: https://ipfs.io/ipfs/QmTkzDwWqPbnAh5YiV5VwcTLnGdwSNsNTn2aDxdXBFca7D/example#/ipfs/QmQwAP9vFjbCtKvD8RkJdCvPHqLQjZfW7Mqbbqx18zd8j7/graphmd/README.md


## D3 Tree

** Status: experimental **

We have adapted a [D3 left-to-right tree example by Mike Bostock](http://mbostock.github.io/d3/talk/20111018/tree.html) for use in visualizing IPFS.

![](https://cdn.rawgit.com/ipfs/dataviz/6021cea7e49224b1bab784ce04e6ef7019be625b/webapps/tree-ltr/doc/ipfs-core.png)

This can be served up via IPFS, and read data from IPFS.  For example,
the tree visualizing its own source code:

https://ipfs.io/ipfs/QmYShjC6KjVPns2AuY77rbDPL1XEygWEo2485r9qL6EYTc/viz#QmYShjC6KjVPns2AuY77rbDPL1XEygWEo2485r9qL6EYTc

The first hash is the visualization; the second hash is whatever is being visualized.

For example, to explore Brewster Kahle's blog, which has the address
`QmavE42xtK1VovJFVTVkCR5Jdf761QWtxmvak9Zx718TVr`, we would visit:

https://ipfs.io/ipfs/QmYShjC6KjVPns2AuY77rbDPL1XEygWEo2485r9qL6EYTc/viz#QmavE42xtK1VovJFVTVkCR5Jdf761QWtxmvak9Zx718TVr

### To install and run it locally:

[Install IPFS](https://ipfs.io/docs/install/)

```
ipfs daemon
git clone git@github.com:ipfs/dataviz.git
cd dataviz/webapps/tree-ltr
make
```

This should load up the tree viz in your browser.
Change the IPFS hash at the end of the URL to see any other IPFS tree.
