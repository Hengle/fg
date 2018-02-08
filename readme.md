- What is a **framegraph**?
  - A directed acyclic graph consisting of **render tasks** and **resources**.
  - A **render task** is a compute or graphics task to be performed on the GPU.
  - A **resource** is data created, modified or used by a **render task**.
    - A **virtual resource** is a resource which has not yet been instantiated but contains all information necessary to do so.
    - A **real resource** is a resource which has been instantiated (by the framegraph or through external means).
    - A **transient** resource is a resource created, realized, unrealized and destroyed by the framegraph. It may be virtual or real.
    - A **retained** resource is a resource which has been imported into the framegraph. It is always real and specified during construction.

- What is next?
  - Render task cull prevention.
  - Asynchronous render task launch (resource barriers).
  - Export to GraphViz.