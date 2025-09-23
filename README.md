# game_of_life_gha

## Game of Life – Java 1.8 with GitHub Actions


## Repository Structure

```
.
├── src/
│   ├── main/java/...        # Game logic and classes
│   └── test/java/...        # Unit tests
├── pom.xml                  # Maven configuration
└── .github/workflows/
    └── build.yaml           # GitHub Actions workflow
```

---


###  Continuous Integration (GitHub Actions)

This repository uses **GitHub Actions** for automated builds and tests. The workflow is defined in:

```
.github/workflows/build.yaml
```

####  How It Works

1. Triggers on:

   * Pushes to `main`.
   * Pull requests targeting `main`.
   * Manual runs via **workflow\_dispatch**.
2. Uses **Ubuntu runners** to:

   * Check out the repository.
   * Install **Java 1.8**.
   * Cache Maven dependencies.
   * Build and test the code.

To view workflow runs: **Actions tab → Build and Test (Java 1.8)**.

---


###  Output

After a successful build, the JAR file will be in the `target/` folder:

```
target/game-of-life-1.0-SNAPSHOT.jar
```

---

###  Author

**Ramani Jadala**

* GitHub: [@jadalaramani](https://github.com/jadalaramani)

---
