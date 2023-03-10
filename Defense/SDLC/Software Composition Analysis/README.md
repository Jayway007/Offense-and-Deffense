## Diagram
```mermaid
graph TD;
    Manifest-->dependency;
    pom.xml-->dependency;
    Appinfo-->dependency;
    dependency-->version;
    dependency-->JarType;
    
    JarType-->opensource;
    Maven-->opensource;
    opensource-->CPE;
    
    NVD-->CVE;
    CPE-->CVE;
    version-->Vulnerability;
    CVE-->Vulnerability;
```

## Tools
- [Dependency-Check](https://github.com/jeremylong/DependencyCheck)
 _Dependency-Check is a Software Composition Analysis (SCA) tool that attempts to detect publicly disclosed vulnerabilities contained within a project's dependencies. It does this by determining if there is a Common Platform Enumeration (CPE) identifier for a given dependency. If found, it will generate a report linking to the associated CVE entries._
- 
