Here’s a concise guide to **frequently asked Maven interview questions** (non-scenario based), ideal for DevOps, Java developer, and build automation roles:

---

## ✅ **Top Maven Interview Questions & Answers**

---

### 🔹 **1. What is Maven?**

**Answer:**
Maven is a **build automation and dependency management tool** primarily for Java projects. It uses a **Project Object Model (POM)** file to manage project structure, dependencies, plugins, and build lifecycle.

---

### 🔹 **2. What is a POM file in Maven?**

**Answer:**
POM (Project Object Model) is an XML file (`pom.xml`) that contains information about the project and configuration details used by Maven to build the project (e.g., dependencies, plugins, build profile).

---

### 🔹 **3. What are the main phases of the Maven build lifecycle?**

**Answer:**

1. `validate` – validate the project is correct.
2. `compile` – compile the source code.
3. `test` – run unit tests.
4. `package` – package code into a `.jar` or `.war`.
5. `verify` – run integration tests.
6. `install` – install package to local repo.
7. `deploy` – deploy to remote repo.

---

### 🔹 **4. What are Maven repositories?**

**Answer:**

1. **Local** – in your machine (`~/.m2/repository`)
2. **Central** – hosted by Maven ([https://repo.maven.apache.org](https://repo.maven.apache.org))
3. **Remote** – custom repositories (e.g., Nexus, Artifactory)

---

### 🔹 **5. What is the difference between `compile`, `provided`, `runtime`, `test`, and `system` scopes in Maven?**

| Scope    | Description                                                                  |
| -------- | ---------------------------------------------------------------------------- |
| compile  | Available everywhere (default scope)                                         |
| provided | Needed for compile but provided at runtime (e.g., servlet-api)               |
| runtime  | Not required for compile, needed at runtime (e.g., JDBC driver)              |
| test     | Only available during test compilation and execution                         |
| system   | Similar to provided, but with explicit path outside of repository management |

---

### 🔹 **6. How do you add a dependency in Maven?**

```xml
<dependency>
  <groupId>org.springframework</groupId>
  <artifactId>spring-core</artifactId>
  <version>5.3.10</version>
</dependency>
```

---

### 🔹 **7. What are Maven plugins?**

**Answer:**
Plugins are used to extend Maven functionality—e.g., compiling code, packaging, running tests.

Example:

* `maven-compiler-plugin`
* `maven-surefire-plugin`

---

### 🔹 **8. What is the difference between `clean`, `install`, and `deploy`?**

* `clean` – deletes the `target/` directory.
* `install` – installs the package to the local repo.
* `deploy` – copies the final package to a remote repository for sharing.

---

### 🔹 **9. How does Maven handle dependency conflicts (transitive dependencies)?**

**Answer:**
Maven uses a **nearest-wins** strategy—if multiple versions exist, the one closest in the dependency tree is used. You can **override** the version explicitly.

---

### 🔹 **10. What is the purpose of the `dependencyManagement` tag?**

**Answer:**
It allows you to define versions for dependencies in parent POMs, so child modules can use them without declaring versions.

---

### 🔹 **11. How do you create a multi-module Maven project?**

* Create a parent POM with `<packaging>pom</packaging>`.
* List modules using:

```xml
<modules>
  <module>service</module>
  <module>web</module>
</modules>
```

---

### 🔹 **12. What are Maven profiles?**

**Answer:**
Profiles allow you to define custom configurations (e.g., dev, test, prod) that activate under specific conditions.

Example:

```xml
<profiles>
  <profile>
    <id>dev</id>
    <activation>
      <activeByDefault>true</activeByDefault>
    </activation>
    ...
  </profile>
</profiles>
```

---

### 🔹 **13. What’s the difference between `build` and `pluginManagement`?**

* `build.plugins` – directly applies the plugin to the current project.
* `pluginManagement` – defines default settings, used only when explicitly referenced.

---

### 🔹 **14. How do you skip tests in Maven?**

```bash
mvn install -DskipTests
```

---

### 🔹 **15. How do you generate a site or documentation in Maven?**

```bash
mvn site
```

---

Would you like me to generate:

* ✅ 10+ **real-time Maven scenario-based interview questions**?
* ✅ A **multi-module Maven project** example?
* ✅ Maven + Jenkins CI integration example?

Let me know how you'd like to continue!
