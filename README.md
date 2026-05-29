# Tableau Dashboard Config Repository

## Overview

This repository stores Tableau Public dashboard configurations in JSON format.

The dashboards are later fetched dynamically by a Java Spring Boot application and displayed automatically.

---

# Architecture

Tableau Public Dashboard
        ↓
Generate Public URL
        ↓
Store URLs in JSON File
        ↓
Push JSON to GitHub
        ↓
Spring Boot Application Reads JSON
        ↓
Display Dashboards Dynamically

---

# Repository Structure

```text
tableau-dashboard-config/
│
├── dashboards.json
├── README.md
```

---

# dashboards.json

This file contains metadata for Tableau dashboards.

Example:

```json
[
  {
    "title": "Sales Dashboard",
    "category": "Sales",
    "description": "Company sales analysis dashboard",
    "url": "https://public.tableau.com/views/SalesDashboard/Sales?:showVizHome=no"
  }
]
```

---

# JSON Fields

| Field | Description |
|------|-------------|
| title | Dashboard title |
| category | Dashboard category |
| description | Dashboard details |
| url | Tableau Public visualization URL |

---

# Purpose of This Repository

This repository acts as:

- Dashboard configuration storage
- Visualization metadata source
- Dynamic dashboard registry
- Centralized BI dashboard management system

---

# Technologies Used

- Tableau Public
- Git
- GitHub
- JSON
- Java Spring Boot
- Thymeleaf

---

# Workflow

1. Create dashboard in Tableau Public
2. Publish visualization
3. Copy Tableau Public URL
4. Add URL inside dashboards.json
5. Push changes to GitHub
6. Spring Boot app automatically reads dashboards

---

# Future Enhancements

- Dashboard categories
- Dashboard search
- REST APIs
- Authentication
- Database integration
- Auto refresh system

---

# Author

Created for dynamic Tableau dashboard integration using Spring Boot.
