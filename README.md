# **AI-Powered Hospital Emergency Detection Chatbot**

An intelligent healthcare assistant built with n8n and OpenAI that provides patient-friendly health guidance, detects medical emergencies in real time, and automatically logs emergency cases into Google Sheets for hospital monitoring and triage management.

---

# **🏥 Overview**

This project simulates a real-world hospital AI assistant that helps patients through a conversational chatbot interface.

The system can:

- Answer general health and wellness questions
- Detect emergency symptoms using AI + intelligent keyword routing
- Categorize emergency types
- Prioritize cases using severity levels
- Automatically track emergency patients in Google Sheets
- Provide instant emergency guidance

---

# **✨ Key Features**

## **🤖 AI Health Assistant**
Provides concise, patient-friendly health guidance for:
- Diet plans
- Wellness tips
- Common symptoms
- Lifestyle recommendations

---

## **🚨 Emergency Detection Engine**
Automatically detects serious symptoms such as:
- Chest pain
- Breathing difficulty
- Stroke symptoms
- Heavy bleeding
- Seizures
- Allergic reactions
- Trauma injuries
- Mental health crises

---

## **📊 Hospital Emergency Monitoring**
Emergency cases are automatically logged into Google Sheets with:
- Timestamp
- Patient message
- Emergency category
- Severity
- Status

This enables hospital staff to monitor critical patients in real time.

---

## **🧠 Smart Triage Logic**
Classifies emergency cases into:
- Cardiac Emergency
- Respiratory Emergency
- Neurological Emergency
- Trauma Emergency
- Mental Health Crisis
- And more...

---

## **⚡ Dynamic Routing**
- Normal health queries → AI assistant response
- Emergency cases → Hospital monitoring workflow

---

# **🧱 Workflow Architecture**

```text
Patient Chat
      ↓
Safety Check & Categorization
      ↓
Emergency Router

TRUE (Emergency)
      ↓
Append Row in Google Sheets
      ↓
Emergency Response

FALSE (Normal)
      ↓
Health Information AI
      ↓
Format Health Response

      ↓
Merge
      ↓
Respond to Chat

# **🛠️ Tech Stack**

| **Technology** | **Purpose** |
|---|---|
| **n8n** | Workflow Automation |
| **OpenAI GPT** | AI Health Assistant |
| **Google Sheets** | Emergency Tracking |
| **JavaScript** | Emergency Detection Logic |
| **Hosted Chat** | Patient Interface |

# **📋 Example Scenarios**

## **✅ Normal Query**

### **Patient:**
suggest BP diet

### **Chatbot:**
Reduce salt intake and avoid processed foods. Eat fruits, vegetables, whole grains, and lean proteins. Stay hydrated and exercise regularly.

---

## **🚨 Emergency Query**

### **Patient:**
can not breath

### **Workflow:**
- Emergency detected
- Google Sheet updated
- Emergency response sent

### **Chatbot:**
🚨 Breathing difficulty may indicate a medical emergency.

Please seek immediate medical attention immediately.


## 📊 Google Sheets Emergency Tracker

| Timestamp | Patient Message | Emergency Type | Severity | Status |
| --- | --- | --- | --- | --- |
| 2026-05-26T11:29:03.298-04:00 | severe chest pain | Cardiac Emergency | Critical | Pending |
| 2026-05-26T11:36:20.375-04:00 | taking breath is difficult | Respiratory Emergency | Critical | Pending |
| 2026-05-26T11:38:35.431-04:00 | suffering with heart pain | Cardiac Emergency | Critical | Pending |
| 2026-05-26T11:41:50.659-04:00 | Met with Accident | Trauma Emergency | High | Pending |
| 2026-05-26T11:42:29.866-04:00 | head injury | Trauma Emergency | High | Pending |
| 2026-05-26T11:43:17.770-04:00 | chest pain | Cardiac Emergency | Critical | Pending |
| 2026-05-26T11:43:58.727-04:00 | heavy bleeding | Bleeding Emergency | High | Pending |
| 2026-05-26T11:44:36.300-04:00 | unconscious | Neurological Emergency | High | Pending |
| 2026-05-26T11:45:47.235-04:00 | drug overdose | Poisoning Emergency | High | Pending |
| 2026-05-26T11:46:35.313-04:00 | cannot breathe | Respiratory Emergency | Critical | Pending |
| 2026-05-26T11:47:40.521-04:00 | chest pain | Cardiac Emergency | Critical | Pending |
| 2026-05-26T11:52:32.558-04:00 | can not breathe | Respiratory Emergency | Critical | Pending |
| 2026-05-26T11:54:42.060-04:00 | stroke i can not walk | Stroke Emergency | Critical | Pending |
| 2026-05-26T12:00:45.073-04:00 | bleeding in brain | Neurological Emergency | High | Pending |
