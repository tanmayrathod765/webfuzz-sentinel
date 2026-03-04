# WebFuzz Sentinel
### Comprehensive Web Application Fuzzer

**Institute:** Shri Vaishnav Institute of Information Technology (SVIIT)  
**Course:** Minor Project 2026  
**Team ID:** WFS-2026-SEC  
**Phase:** Phase 1 - Planning & Requirement Analysis  

---

## Project Overview
WebFuzz Sentinel is an automated web application security 
reconnaissance platform that identifies vulnerabilities across 
directories, virtual hosts, API endpoints, URL parameters, 
and subdomains before attackers do.

---

## Project Structure
```
webfuzz-sentinel/
├── src/
│   ├── modules/       # Fuzzing modules (dir, vhost, api, param, subdomain)
│   ├── engine/        # Core HTTP request engine
│   ├── classifier/    # Vulnerability classification logic
│   ├── reporter/      # Report generation
│   └── visualizer/    # Frontend components
├── wordlists/         # Built-in wordlists and payloads
├── tests/             # Unit and integration tests
├── docs/              # Documentation and UML diagrams
└── config/            # Configuration files
```

---

## Team
| Role | Responsibility |
|------|---------------|
| Project Lead | Sprint planning, stakeholder communication |
| Security Engineer | Module design, vulnerability logic |
| Frontend Developer | UI, radar visualization, neural map |
| Backend Developer | HTTP engine, reporting |
| QA Engineer | Testing, false positive analysis |
| DevOps | Git, Jira, CI/CD pipeline |

---

## Timeline
- **Phase 1** (Weeks 1-2): Planning & Requirement Analysis
- **Phase 2** (Weeks 3-4): Object-Oriented Analysis
- **Phase 3** (Weeks 5-7): Object-Oriented Design
- **Phase 4** (Weeks 8-10): Implementation & CI/CD
- **Phase 5** (Weeks 11-12): Testing & Deployment
```

4. **"Commit changes"** click karo

---

### Step 4 — Branches Banao

**develop branch banana:**
1. Repo mein jao
2. **"main"** dropdown click karo (top left)
3. Search box mein likho: `develop`
4. **"Create branch: develop from main"** click karo

**feature branch banana:**
1. Wahi dropdown mein likho: `feature/project-init`
2. **"Create branch: feature/project-init from develop"** click karo

**docs branch banana:**
1. Wahi dropdown mein likho: `docs/phase1-planning`
2. **"Create branch: docs/phase1-planning from develop"** click karo

---

### Step 5 — Branch Protection Lagao

**main branch protect karo:**
1. Repo → **Settings** tab
2. Left menu → **Branches**
3. **"Add branch protection rule"** click karo
4. Branch name pattern mein likho: `main`
5. Yeh tick karo:
```
✅ Require a pull request before merging
✅ Require approvals (1)
✅ Require status checks to pass
```
6. **"Create"** click karo

**develop ke liye bhi same karo** — branch name mein `develop` likho

---

## PART 2 — Jira Setup (20 min)

### Step 1 — Project Banao

1. `jira.atlassian.com` kholo
2. **"Create project"** click karo
3. **"Scrum"** select karo → Next
4. Yeh fill karo:
```
Project name:  WebFuzz Sentinel
Project key:   WFS
```
5. **"Create"** click karo

---

### Step 2 — Team Members Add Karo

1. Project settings → **"People"**
2. **"Add people"** click karo
3. Team members ki email daalo ek ek karke
4. Role: **"Member"** rakho sabke liye
5. Project Lead ko **"Admin"** banao

---

### Step 3 — Epics Banao

Left menu mein **"Backlog"** click karo. Phir **"Create Epic"** karo — yeh 10 epics banao ek ek:
```
Epic 1:  Directory Fuzzer           → Label: CRITICAL  → Component: DIR
Epic 2:  VHost Discovery            → Label: HIGH      → Component: VHOST
Epic 3:  API Endpoint Detection     → Label: CRITICAL  → Component: API
Epic 4:  Parameter Fuzzing          → Label: CRITICAL  → Component: PARAM
Epic 5:  Subdomain Enumeration      → Label: HIGH      → Component: SUBDOMAIN
Epic 6:  Threat Radar UI            → Label: MEDIUM    → Component: UI
Epic 7:  Neural Attack Map          → Label: MEDIUM    → Component: UI
Epic 8:  Classification Engine      → Label: HIGH      → Component: CORE
Epic 9:  Reporting & Export         → Label: HIGH      → Component: REPORT
Epic 10: Custom Wordlists           → Label: MEDIUM    → Component: CORE
```

---

### Step 4 — Sprint 1 User Stories Banao

Backlog mein **"Create issue"** click karo — type **"Story"** — yeh 7 stories banao:
```
Story 1:
  Title:       Set up project repo, CI pipeline, and dev environment
  Epic:        Classification Engine
  Points:      3
  Assignee:    DevOps

Story 2:
  Title:       Implement core HTTP request engine with configurable concurrency
  Epic:        Directory Fuzzer
  Points:      8
  Assignee:    Backend Developer

Story 3:
  Title:       Build directory enumeration module using built-in wordlist
  Epic:        Directory Fuzzer
  Points:      5
  Assignee:    Security Engineer

Story 4:
  Title:       Implement response classifier (status, size, time heuristics)
  Epic:        Classification Engine
  Points:      5
  Assignee:    Security Engineer

Story 5:
  Title:       Create basic results table UI with status and URL columns
  Epic:        Threat Radar UI
  Points:      3
  Assignee:    Frontend Developer

Story 6:
  Title:       Write unit tests for HTTP engine and classifier modules
  Epic:        Classification Engine
  Points:      3
  Assignee:    QA Engineer

Story 7:
  Title:       Implement JSON export for scan results
  Epic:        Reporting & Export
  Points:      2
  Assignee:    Backend Developer
```

---

### Step 5 — Sprint Banao

1. Backlog mein upar **"Create sprint"** click karo
2. Sprint pe click karo → **"Edit sprint"**
3. Yeh fill karo:
```
Sprint name:  Sprint 1
Start date:   19 Jan 2026
End date:     31 Jan 2026
Sprint goal:  Set up project infrastructure, define product backlog, 
              and complete Phase 1 planning documentation
```
4. Saari 7 stories ko sprint mein drag karo
5. **"Start sprint"** click karo

---

## PART 3 — Team Ko Roles Assign Karo

Team members ko batao kaun kya karega. Yeh WhatsApp/group mein share karo:
```
WebFuzz Sentinel — Team Roles

[Tumhara naam]     → Project Lead
[Team member 2]    → Security Engineer  
[Team member 3]    → Frontend Developer
[Team member 4]    → Backend Developer
[Team member 5]    → QA Engineer
[Team member 6]    → DevOps Engineer

GitHub Repo: github.com/[tumhara-username]/webfuzz-sentinel
Jira Board:  [tumhari jira link]
```

---

## Sab Ho Gaya? Checklist

Yeh sab check karo:
```
GitHub:
  ☐ Repository bani — webfuzz-sentinel
  ☐ Sab folders bane — src, wordlists, tests, docs, config
  ☐ README.md updated
  ☐ 3 branches bani — main, develop, feature/project-init
  ☐ Branch protection laga — main aur develop pe

Jira:
  ☐ Project bana — WebFuzz Sentinel (WFS)
  ☐ Team members added
  ☐ 10 Epics bane
  ☐ 7 User Stories bani
  ☐ Sprint 1 bana aur start kiya

Team:
  ☐ Sabko roles pata hain
  ☐ GitHub repo access diya
  ☐ Jira access diya
