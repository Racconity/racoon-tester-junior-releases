# 🦝 Racoon Tester Junior

**A desktop quality studio for developers.**

Discover, organize, run, and inspect automated tests across your projects—from one place.

Racoon Tester Junior began as a simple way to explore Go and TypeScript tests without jumping between terminals and directories. It has grown into a lightweight desktop workspace for test execution, code-quality checks, and end-to-end demonstrations.

> **Status:** Early release. Features and compatibility may evolve as the application matures.

## ✨ Features

- **Test Explorer:** Browse discovered Go, Vitest, and Playwright tests across multiple project folders.
- **Test execution:** Run supported suites and individual tests, review results, and cancel running processes.
- **Coverage Studio:** Inspect coverage results using supported project tooling.
- **Code Inspector:** Run supported static-analysis and linting checks.
- **Quality Profiles:** Save reusable sequences of quality checks.
- **History:** Review previous runs and their outcomes.
- **Evidence Studio:** Browse screenshots, videos, and traces produced by supported Playwright executions; open traces using Playwright's own viewer.
- **Demo Studio:** Run real E2E scenarios in sequence, with headed browser playback and supported controls for speed, viewport, and timeouts.
- **Personalization:** English and Spanish UI, with Dark and Racoonity themes.

Junior orchestrates existing tools. It does **not** replace your test frameworks or automatically create tests for your projects.

## 📦 Download and install

1. Open this repository's **[Releases](../../releases)** page.
2. Download the Windows installer or application package provided with the latest release.
3. Install and launch **Racoon Tester Junior**.
4. Add your project folders to the workspace and let Junior discover supported tests.

**Platform:** Windows is the initial distribution target. Other platforms are not currently advertised as supported.

> **Windows SmartScreen:** Early unsigned builds may trigger a reputation warning. Confirm the file comes from this repository's official Releases page before deciding whether to run it. Never bypass a security warning for a file you do not trust.

## 🧰 Requirements

Junior does not bundle every development tool your projects might need. Depending on which features you use, install and configure the relevant tools in your environment:

| Feature | Typical project-side requirement |
| --- | --- |
| Go tests | Go toolchain |
| TypeScript / JavaScript tests | Node.js and project dependencies (such as Vitest) |
| Playwright E2E | Project-local Playwright Test and browser binaries |
| Coverage and code inspection | The corresponding project's supported coverage or lint tooling |
| External E2E harnesses | Their own runtimes, environment variables, and supporting services |

Some test suites need databases or other services. Junior does not provision those automatically unless the project's existing test harness does so.

## 🚀 Quick start

1. Select **Add Folder / Agregar carpeta**.
2. Add one or more folders containing supported projects.
3. Open the **Tests** tab to browse discovered suites.
4. Run a test or suite and inspect the results.
5. Explore **Coverage**, **Inspector**, **Profiles**, **History**, **Evidence**, or **Demo** as needed.

Available actions depend on the detected framework and the project's configuration.

## 🎬 Playwright and E2E demonstrations

Junior can work with Playwright projects and can also launch E2E journeys through an externally configured harness. For example, an external Go harness may be responsible for preparing a test database, starting an API and frontend, and then launching Playwright.

Demo controls such as browser visibility, slow motion, viewport size, evidence capture, and test timeout are applied only when supported by the corresponding runner or harness. **Opening a project does not imply that its E2E environment is ready to run.**

E2E tests may modify the application and its data. Run them only against controlled test environments.

## 🔐 Privacy and safety

- Junior operates locally; it is not a hosted testing service.
- Test execution runs code from the projects you choose. Only open and run projects you trust.
- Test logs, screenshots, videos, and traces may contain credentials or sensitive information. Review them before sharing.
- E2E execution may require explicit environment configuration, external services, and project-specific safeguards.

## 🐛 Issues and feedback

Found a bug or have an idea? Open an **[Issue](../../issues)** in this repository.

When reporting a problem, please include the Junior version, Windows version, relevant framework, reproduction steps, and a sanitized error message or screenshot. **Do not post secrets, database URLs containing passwords, or sensitive traces.**

## 📄 Repository scope

This is the **public release and feedback repository** for Racoon Tester Junior. The application's source code is maintained separately and is **not published here**.

Public download availability does not grant permission to redistribute, modify, or relicense proprietary application code. Check the applicable release terms before redistributing packages.

## 🦝 Part of the Racoonity ecosystem

Racoon Tester Junior is an independent developer tool created alongside **[Racoonity](https://racoonity.com/)**. It can be used with other compatible projects; Racoonity is not required.

*Small tool. Big ambitions.*
