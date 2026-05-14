# 🏗️ Land Development eDA
### Business Process Management Application — Bonita BPM Platform

![Bonita BPM](https://img.shields.io/badge/Bonita-BPM-orange?logo=java&logoColor=white)
![Java](https://img.shields.io/badge/Java-Maven-red?logo=apachemaven&logoColor=white)
![Forms](https://img.shields.io/badge/Forms-12%20Workflows-blue)
![GIS](https://img.shields.io/badge/GIS-Integrated-green)
![i18n](https://img.shields.io/badge/Localization-AR%20%7C%20EN-purple)

> **Course:** Business Process Management — King Khalid University  
> **Author:** Rana Sultan Alhinidy

---

## 📋 Overview

A fully automated **Land Development permit management system** built on the Bonita BPM platform. The application digitizes the end-to-end workflow for processing land development permit applications — from initial submission through GIS validation, cost quoting, review, and final licence issuance.

---

## ✨ Key Features

| Feature | Details |
|---|---|
| 🔄 **Full BPM Workflow** | End-to-end automated process for land permit applications |
| 📋 **12 Smart Forms** | Dynamic UI forms covering every stage of the process |
| 🗺️ **GIS Integration** | Geospatial data retrieval for land location validation |
| 🌍 **Bilingual Support** | Full Arabic & English localization (i18n) |
| ⚙️ **Multi-Environment** | Separate Production & Qualification configurations |
| 🏗️ **Maven Build** | Professional Java/Groovy project structure |

---

## 🔄 Process Workflow

The system automates the full permit lifecycle:

```
Applicant                    Municipality                      GIS / Finance
   │                              │                                 │
   ├─── Submit Application ──────►│                                 │
   │                              ├─── Receive & Validate ──────────┤
   │                              │◄── Retrieve GIS Data ───────────┤
   │                              ├─── Review for Validation        │
   │                              ├─── Check Road Conflicts ────────┤
   │                              ├─── Prepare Cost Quote           │
   │◄── Receive Quote ────────────┤                                 │
   ├─── Apply / Pay ─────────────►│                                 │
   │                              ├─── Send DMR                     │
   │                              ├─── Issue Permit                 │
   │◄── Receive Final Decision ───┤                                 │
   │◄── Issue Licence ────────────┤                                 │
```

---

## 📂 Project Structure

```
land_development_eda/
│
├── app/
│   ├── pom.xml                        ← Maven build configuration
│   ├── diagrams/
│   │   └── smartEDA_organization.proc ← BPM process diagram
│   ├── environements/
│   │   ├── Production.xml             ← Production environment config
│   │   └── Qualification.xml          ← Testing environment config
│   └── web_page/
│       ├── SubmitApplicationForm/     ← Applicant submission form
│       ├── receiveApplicationForm/    ← Municipality intake form
│       ├── retriveGISForm/            ← GIS data retrieval form
│       ├── reviewforValidationForm/   ← Technical review form
│       ├── checkRoadConflictsForm/    ← Road conflict check form
│       ├── prepareCostQuoteForm/      ← Cost estimation form
│       ├── receiveQuoteForm/          ← Applicant quote receipt
│       ├── applyAdditionalfeeForm/    ← Additional fees form
│       ├── sendDMRForm/               ← DMR submission form
│       ├── issuePermitForm/           ← Permit issuance form
│       ├── receiveFinalForm/          ← Final decision receipt
│       ├── issueLicenceForm/          ← Licence issuance form
│       └── rejectionForm/             ← Rejection notification form
```

---

## 🧩 Technology Stack

| Layer | Technology |
|---|---|
| **BPM Platform** | Bonita BPM (Bonita Studio) |
| **Backend Language** | Groovy (JVM) |
| **Build Tool** | Apache Maven |
| **UI Forms** | Bonita UI Designer (JSON-based) |
| **GIS** | Integrated geospatial data connector |
| **Localization** | JSON-based i18n (Arabic & English) |
| **Deployment** | Multi-environment (Production / Qualification) |

---

## 📋 Forms Overview

| Form | Stage | Description |
|---|---|---|
| `SubmitApplicationForm` | 1 — Apply | Applicant fills land development request |
| `receiveApplicationForm` | 2 — Intake | Municipality receives and logs the application |
| `retriveGISForm` | 3 — GIS | Fetches geospatial data for the land parcel |
| `reviewforValidationForm` | 4 — Review | Technical team validates the application |
| `checkRoadConflictsForm` | 5 — Conflicts | Checks for road and infrastructure conflicts |
| `prepareCostQuoteForm` | 6 — Quote | Finance team prepares the cost estimate |
| `receiveQuoteForm` | 7 — Payment | Applicant reviews and accepts the quote |
| `applyAdditionalfeeForm` | 8 — Fees | Applies any additional fees if required |
| `sendDMRForm` | 9 — DMR | Sends the Development Management Report |
| `issuePermitForm` | 10 — Permit | Issues the development permit |
| `receiveFinalForm` | 11 — Final | Applicant receives the final decision |
| `issueLicenceForm` | 12 — Licence | Official licence is issued |
| `rejectionForm` | — | Handles rejection at any stage |

---

## 🚀 Getting Started

### Prerequisites
- [Bonita Studio](https://www.bonitasoft.com/downloads) (Community or Enterprise)
- Java 11+
- Apache Maven 3.6+

### Setup

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/land-development-eda.git
cd land-development-eda

# 2. Open in Bonita Studio
# File → Import → BOS file → select the .bos file

# 3. Or build with Maven
mvn clean install
```

### Importing the Process
1. Open **Bonita Studio**
2. Go to **File → Import → BOS Archive**
3. Select `land_development_eda.bos`
4. Deploy to your local Bonita server

---

## 🎓 Academic Context

**Course:** Business Process Management  
**University:** King Khalid University  
**Concepts demonstrated:**
- ✅ BPM process modeling and automation
- ✅ Multi-actor workflow design
- ✅ Form-driven UI with dynamic validation
- ✅ GIS data integration
- ✅ Multi-environment deployment configuration
- ✅ Bilingual (AR/EN) application design

---

## 📄 License

This project was developed for academic purposes at King Khalid University.
