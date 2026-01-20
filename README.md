## Demo Project Overview

This repository is a demonstration project that includes two main components: **Generation (Gen)** and **Fitting (Fit)**.
The workflow is executed using **REANA** as the runner backend.

An introduction to this example is also available on **Read the Docs**.

---

## Steps to Run the Example

### 1. Clone the Repository

```bash
git clone <repo-url>
cd demo-basic-01
```

### 2. Enter the Celebi Environment

```bash
celebi use .   # Use the this legacy project
celebi
```

You are now inside the **Celebi shell**.

### 3. Verify DITE Connection

List the current status:

```bash
ls
```

If DITE is not connected, you will see something other than:

```text
>>>> DITE: [connected]
```

To check the DITE:

```bash
dite
```

Configure the DITE endpoint (only required once):

```bash
set-dite https://dite.reana.io/
```

### 4. Check Available Runners

```bash
runners
```

If no runner is registered, register one:

```bash
register-runner
```

### 5. Submit the Workflow

```bash
submit
```
