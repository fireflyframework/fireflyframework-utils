# Firefly Framework - Utilities

[![CI](https://github.com/fireflyframework/fireflyframework-utils/actions/workflows/ci.yml/badge.svg)](https://github.com/fireflyframework/fireflyframework-utils/actions/workflows/ci.yml)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Java](https://img.shields.io/badge/Java-21%2B-orange.svg)](https://openjdk.org)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-green.svg)](https://spring.io/projects/spring-boot)

> Utility library providing template rendering, PDF generation, and filtering annotations for Firefly Framework applications.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Quick Start](#quick-start)
- [Configuration](#configuration)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Overview

Firefly Framework Utilities provides a set of common utility classes used across the framework ecosystem. It includes template rendering powered by FreeMarker, PDF generation via Flying Saucer with OpenPDF, and filtering annotations for domain entity identification.

This library is a lightweight foundation module with minimal dependencies, designed to be included wherever utility functions are needed without pulling in the full framework stack.

## Features

- Template rendering with FreeMarker via `TemplateRenderUtil`
- PDF generation using Flying Saucer and OpenPDF
- `@FilterableId` annotation for marking domain entity identifiers
- Lightweight with minimal transitive dependencies

## Requirements

- Java 21+
- Spring Boot 3.x
- Maven 3.9+

## Installation

```xml
<dependency>
    <groupId>org.fireflyframework</groupId>
    <artifactId>fireflyframework-utils</artifactId>
    <version>26.02.02</version>
</dependency>
```

## Quick Start

```java
import org.fireflyframework.utils.template.TemplateRenderUtil;

// Render a FreeMarker template
Map<String, Object> data = Map.of("name", "Firefly");
String result = TemplateRenderUtil.render("hello.ftl", data);
```

## Configuration

No configuration is required. This library provides standalone utility classes.

## Documentation

No additional documentation available for this project.

## Contributing

Contributions are welcome. Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide for details on our code of conduct, development process, and how to submit pull requests.

## License

Copyright 2024-2026 Firefly Software Solutions Inc.

Licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for details.
