# 🏥 Telemedicine Digital Twin Architecture (PSM)

This repository contains the architectural and conceptual models for a **Digital Twin** and **Telemonitoring System** applied to telemedicine. The project focuses on the system administration, clinical evaluation workflows, and patient interactions.

The models are provided as `.drawio` diagrams, along with a final presentation (`RELAZIONE FINALE.pptx`). 

---

## 📋 System Overview

The system bridges a **Telemonitoring Platform**, a **Specialized Electronic Health Record (Cartella Specialistica)**, and a **Patient Digital Twin App**. It is designed to assist doctors in tracking patient data and alerts, while providing patients with a straightforward interface to log their daily symptoms.

### Key Workflows Modeled:
1. **Clinical Area Workflow (Doctor's view)**:
   - **Form 1 (Patient Clinical Data)**: The doctor selects a patient to view their clinical records and import new monitoring data.
   - **Form 2 (Clinical Status Evaluation)**: A weekly dashboard showing sensor data (BPM, pressure, SpO2), manual patient inputs (temperature, weight), word clouds of symptoms, and alert levels. The doctor can validate the patient's status as "Stable" or "Altered" and add clinical notes.

2. **Digital Twin App (Patient's view)**:
   - **Clinical Diary**: Patients can log how they feel and describe symptoms.
   - **Manual Monitoring**: Allows manual entry of temperature, weight, and symptom scales.
   - **Notes**: Free text entry for additional context.
   - All entries require explicit confirmation before being synchronized with the Specialized EHR.

3. **System Integration & Synchronization**:
   - **Data Exchange**: Synchronization between the Digital Twin and the Specialized EHR ensures that the doctor always analyzes the latest patient data.
   - **Alert System**: An automated process that analyzes incoming clinical data against therapeutic ranges. It generates risk levels for each day and emits alerts if data reception fails or if biological parameters are out of bounds.
   - **Aggregated Data Transfer**: Packets of aggregated sensor data are validated and sent from the telemonitoring platform to both the Digital Twin and the Specialized EHR.

---

## 📂 Repository Contents

- **`*.drawio` Diagrams**: Contains various UML, Communication, Activity, Entity, and Process diagrams detailing every system interaction.
    - `ACTIVITY - SOFTWARE.drawio`, `ACTIVITY INTERFACCIE.drawio`
    - `COMMUNICATION_DIAGRAM.drawio`
    - `Object Entity.drawio`
    - `PROCESSO 1-5.drawio`
    - `Consulta_dati.drawio`, `ESERCITAZIONE.drawio`, `UML.drawio`
- **`RELAZIONE FINALE.pptx`**: Final project presentation.

*(Note: Peer review documents and internal drafts are intentionally excluded from this repository).*

---
*Created as an academic modeling project (PSM).*
