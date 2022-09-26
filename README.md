# Mentcare Case Study - cited from Ian Sommerville Software Engineering, Tenth Edition 

https://software-engineering-book.com/case-studies/

This case study is part of the Open Design Case Study project. This work is licensed under the Creative Commons Attribution-NonCommercial 3.0 ([CC BY-NC 3.0](https://creativecommons.org/licenses/by-nc/3.0/us/)) United States License.

### Citation

Sommerville, I. (2016) Software Engineering. 10th Edition, Pearson Education Limited, Boston.

### Title

Mentcare: A mental health support system

### Objectives

The patient information system to support mental health care (the Mentcare system) is a medical information system that maintains information about patients suffering from mental health problems and the treatments that they have received.  The system is designed for use in clinics attended by patients suffering from mental health problems and records details of their consultations and conditions. It is separate from a more general patient records system as more detailed information has to be maintained and the system has to be set up to generate letters and reports of different types and to help ensure that the laws pertaining to mental health are maintained by staff treating patients.

### Stakeholder

- Clinical staff 
- Doctors
- Hospital administrator
- System administrator
- Health service manager (do not use system, but will request for report generation)
- Mental Health Act administrator (government official to arrange and manage all mental health assessments)

### Requirements

#### Description

1. Individual care management - Clinicians can create records for patients, edit theinformation in the system, view patient history, etc. The system supports data summaries so that doctors who have not previously met a patient can quickly learn about the key problems and treatments that have been prescribed
2. Patient monitoring - The system regularly monitors the records of patients that areinvolved in treatment and issues warnings if possible problems are detected. Therefore, if a patient has not seen a doctor for some time, a warning may be issued. One of themost important elements of the monitoring system is to keep track of patients who have been sectioned(detained in a secure hospital without their consent) and to ensure thatthe legally required checks are carried out at the right time.
3. Managing involuntary detention - In a minority of cases, patients may be a danger tothemselves or to other people. They may regularly change address and may behomeless on a long-term or short-term basis. Where patients are dangerous, they may need to be ‘sectioned’–confined to a secure hospital for treatment and observation. The system must make provision for managing patients who have been detained and for ensuring that all required legal processes are followed and documented

Detailed requirements can be found [here](https://www.dropbox.com/s/61a7hg7tbw4p0nx/Mentcare%20requirements%20document.pdf?dl=0)

#### Constraints

1. The safety implications stem from the fact that some mental illnesses cause patients tobecome suicidal or a danger to other people. Wherever possible, the system should warn medical staff about potentially suicidal or dangerous patients. Other safety issues concern checking of drug dosage and appropriate medication.
2. The system must be available when needed otherwise safety may be compromised and it may be impossible to prescribe the correct medication to patients.
3. As in all medical systems, privacy is a critical system requirement. It is essential that patient information is confidential and is never disclosed to anyone apart from authorized medical staff and the patient themselves. Hospital managers should not have access to individual patient information.
4. The Mentcare system shall run on hardware (Linux servers) that is available in the authority’s data centre. Note that the maximum server memory available is currently 32GB.

#### Quality Attributes

1. Usability -  (a) can learn to use the system quickly; (b) can use the system without undue effort during a patient consultation; (c) make as few errors as possible when using the system
2. Availability - The Mentcare system shall be continuously available during ‘normal’ clinic working hours between 0800 and 1830, Monday to Friday
3. Performance - The system shall normally respond to all user queries about an individual within 2 seconds. If a system response is greater than 2 seconds, then the system shall display an indicator to the user that processing is taking place. This avoids user frustration if there has been a system failure and they keep waiting for a response that does not arrive.

### Environment

#### Entities and Assumptions

| Entities  | Assumptions  |
|---|---|
|  Clinical Staff | Interact directly with the system, looking up and modifying patient information. They are particularly concerned with maintaining a history of consultations and recording the treatment and medication prescribed to patients  |
| Hospital Administrator | Interact directly with the system and use it in conjunction with a generic appointments system to record information about patient appointments. They need to record when appointments were made, the appointment date and whether or not patients attended appointments. Administrators are also responsible for generating reports for clinic management. |
| System Administrator  | System administrators are responsible for ensuring the security and integrity of the system. They are also responsible for integrating the system with other patient record systems, sharing information when required. |
| Records Manager | Medical records managers are responsible for ensuring that the system conforms to legal requirements on personal information systems. The medical records office is responsible for ensuring the overall integrity and security of the data in the system.|

### Design Solution

Not available on the case study - contributors are encourage to suggest their design solution(s)


### Teaching Materials

#### Suggested Usage

1. The author use this case study to discuss general issues of around the requirements for information systems where the system dependability is important and security is a significant concern. It is particularly useful for highlighting requirements conflicts as there is a clear conflict between requirements for patient privacy and safety requirements for maintaining the safety of the patient and their carers.
2. The case study is also useful in any course on requirements engineering as a complete requirements document for the system is available. This illustrates how requirements documents may be organized and can be used as a basis for discussing the issues and problems in developing requirements documents.

### Other notes and resources

- The following paper describes an approach to requirements engineering that was developed to take account of system-wide dependability and security requirements. 
- This uses examples from the system from which the Mentcare requirements were defined. 
- The presentation discusses the use of this approach in deriving requirements for the Mentcare system.

[Dependability Requirements Engineering](https://www.dropbox.com/s/ffj12h421nfqzk1/DependabilityReqEngineering.pdf?dl=0)


[Deriving Dependability Requirements](https://www.dropbox.com/s/8t84unls2ddvi53/Deriving%20dependability%20requirements.pdf?dl=0)
