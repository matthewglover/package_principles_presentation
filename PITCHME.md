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
#### 1. Cohesion: The Reuse-Release Equivalence Principle (REP)
 _The granule of reuse is the granule of release._
 - packages released, versioned and tracked
 - package user should be able to choose when/if to update
 - See semver.org
---
#### 2. Cohesion: The Common-Reuse Principle (CRP)
 _The classes in a package are reused together. If you resuse one of the classes in a package, you reuse all of them._
 - identifies classes which shouldn't be together
 - classes in a package should be inseperable
---
#### 3. Cohesion: The Common-Closure Principle (CCP)
 _The classes in a package should be closed together against the same kind of changes. A change that affects a package affects all the classes in the package and no other package._
 - Single-Responsibility Principle for packages
 - Package should not have multiple reasons to change
 - Tightly bound to Open-Closed Principle
 - Changes should not cross package boundaries
---
### Principles of Package Coupling
 - Relationships between packages
 - Developability vs Logical Design
---
### 4. Coupling: The Acyclic-Dependencies Principle (ADP)
 _Allow no cycles in the package dependencies graph_
  - cycles mean change to any package affects all packages
  - easier to isolate package for testing purposes
---
### 5. Coupling: The Stable-Dependencies Principle (SDP)
 _Depend in the direction of stablility_
  - stability = higher cost of change (many dependents)
  - irresponsible and dependent vs responsible and independent
---
### 6. Coupling: Stable Abstractions Principle
 _A package should be as abstract as it is stable_
 - stable packages should be more abstract
 - abstract classes can be extended without need for modification
 
 
