---
# Principles of Package Design
---
### Background
 - Robert C Martin
 - Agile Software Development _Principles Patterns, and Practices_
 - High level application structure and design
 - x6 Principles:
  - x3 re package cohesion (granularity)
  - x3 re package coupling
---
### Principles of Package Cohesion
 - How to partition Classes into Packages
 - Bottom-up view of partitioning
---
#### 1. The Reuse-Release Equivalence Principle (REP)
 _The granule of reuse is the granule of release_
 - packages released, versioned and tracked
 - package user should be able to choose when/if to update
 - See Semantic Versioning
---
#### 2. The Common-Reuse Principle (CEP)
 _The classes in a package are reused together. If you resuse one of the classes in a package, you reuse all of them_
 - identifies classes which shouldn't be together
 - classes in a package should be inseperable
---
#### 3. The Common-Closure Principle (CCP)
