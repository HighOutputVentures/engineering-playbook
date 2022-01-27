# Continuous Integration

Continuous integration (CI) is the practice of integrating changes from multiple contributors into a single codebase, a single project perhaps, and ensuring the health of the software through running checks with every change. This allows us to reduce our assumptions about our changes by getting feedback early through a repeatable integration process. You can see the effect of your changes brings to the overall project immediately and do decisions accordingly after.

### 🥅 Goals

1. Every change in the codebase goes through the same code checks before merging.
2. Get the entire team to commit with the selected code checks that the team decided.
3. Streamline Pull Requests by catching trivial code issues that can be automated through tools.



### Master CI Pipeline

1. Run a **Code Inspection Tool** to enforce coding conventions on the fly, every language nowadays  has its own community lint support, for typescript we use **ESLint**.
2. Run all available tests, we usually do API testing for Backend.
3. Build all artifacts needed for deployment usually a **docker** image
4. Deploy the artifact generated on the specified platform, e.g. **Kubernetes**
5. Run all kinds of data migrations and post-deployment scripts

### Feature CI Pipeline

1. Run a **Code Inspection Tool** to enforce coding conventions on the fly, every language nowadays has its own community lint support, for typescript we use **ESLint**.
2. Run all available tests, we usually do API testing for Backend.

For feature branches we are limited to steps 1 & 2 unless there are special cases, we can always add steps in the pipeline.
