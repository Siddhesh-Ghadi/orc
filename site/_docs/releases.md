---
layout: docs
title: Releases
permalink: /docs/releases.html
---

## Current Release - 1.2.0:

ORC 1.2.0 contains both the Java reader and writer and the C++ reader for ORC files. It also
contains tools for working with ORC files and looking at their contents and
metadata.

* Released: 25 August 2016
* Source code: [orc-1.2.0.tar.gz]({{site.dist_mirror}}/orc-1.2.0/orc-1.2.0.tar.gz)
* [GPG Signature]({{site.dist}}/orc-1.2.0/orc-1.2.0.tar.gz.asc)
  signed by [Owen O'Malley (3D0C92B9)]({{site.dist}}/KEYS)
* Git tag: [d71f1338]({{site.tag_url}}/release-1.2.0)
* SHA 256: [5c394c7e]({{site.dist}}/orc-1.2.0/orc-1.2.0.tar.gz.sha256)

The new features of ORC 1.2:

- [ORC-54]({{site.jira}}/ORC-54) Evolve schemas based on field name rather than index
- [ORC-84]({{site.jira}}/ORC-84) Create a separate java tool module.
- [ORC-77]({{site.jira}}/ORC-77) and [ORC-81]({{site.jira}}/ORC-81) Implement LZO and LZ4 compression codecs.
- [ORC-92]({{site.jira}}/ORC-92) Add support for nested column id selection in C++
- [ORC-69]({{site.jira}}/ORC-69) Add batch option support in orc-scan tools.

Important fixes:

- [HIVE-14214]({{site.jira}}/HIVE-14214) ORC schema evolution and predicate push down do not work together.

Known issues:

- [ORC-40]({{site.jira}}/ORC-40) Predicate push down is not implemented in C++.

## Checking signatures

All GPG signatures should be verified as matching one of the keys in ORC's
committers' [key list]({{ site.dist }}/KEYS).

~~~ shell
% shasum -a 256 orc-X.Y.Z.tgz | diff - orc-X.Y.Z.tgz.sha256
% gpg --import KEYS
% gpg --verify orc-X.Y.Z.tgz.asc
~~~

## Previous releases:

| Version | Date        | Release   |
| :-----: | :---------: | :-------: |
| 1.1.2   |  8 Jul 2016 | [ORC-1.1.2]({{site.url}}/news/2016/07/08/ORC-1.1.2/)|
| 1.1.1   | 13 Jun 2016 | [ORC-1.1.1]({{site.url}}/news/2016/06/10/ORC-1.1.1/)|
| 1.1.0   | 10 Jun 2016 | [ORC-1.1.0]({{site.url}}/news/2016/06/10/ORC-1.1.0/)|
| 1.0.0   | 25 Jan 2016 | [ORC-1.0.0]({{site.url}}/news/2016/01/25/ORC-1.0.0/)|