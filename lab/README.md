# ContextQA lab — Java · Spring MVC / JSP

Educational source fork of [spring-petclinic/spring-framework-petclinic](https://github.com/spring-petclinic/spring-framework-petclinic). Original history, notices and license are retained. This is not an endorsed integration or a customer production app.

**Status: source and exercises available. Public deployment, platform import and ContextQA run results are not verified.**

Starting source commit: `cf392920cdbe9cd07689f1f4b603271940bac957`.

## Setup and scope

Follow upstream build/runtime prerequisites. Older architecture does not imply an unsupported old Java runtime. Compare the same business assertions with the Spring Boot PetClinic track after independently seeding each app.

Follow the [original setup instructions](../README.md#upstream-project-documentation). See [stack/platform guidance](https://github.com/contextqaai/testing-lab/blob/main/PLATFORMS.md) for deployment boundaries.

## Exercises

| Scenario | Explicit assertion |
|---|---|
| Owner search | A seeded owner is found by the specified name. |
| Required fields | The selected invalid owner form is rejected. |
| Pet creation | The new pet is associated with the selected owner. |
| Visit | The saved visit belongs to the intended pet. |
| Migration parity | Equivalent owner/pet/visit outcomes hold in both configured PetClinic variants. |

These are acceptance exercises, not claims that upstream currently satisfies each desired requirement. Inspect the implemented workflow and fixtures before generating executable steps. Missing validation/auth may deliberately demonstrate a failure and must be disclosed.

## End-to-end lesson

Start an owned/authorized copy with synthetic fixtures. State the assertion, create/review a test in your authenticated ContextQA workspace, execute, and inspect the actual verdict. Introduce one disclosed regression in a separate variant, rerun the same assertion, fix the app and rerun. Confirm mutations against disposable data. Keep credentials and private reports out of this repository.

Record app commit/build, fixture/scenario version, browser/runner version, environment and timestamp with every real report. A cached report is recorded evidence, not a new run. No ContextQA report has been generated for this fork yet.

[ContextQA setup](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) · [Central catalog](https://github.com/contextqaai/testing-lab)
