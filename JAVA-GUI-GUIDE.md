# GUVI HCL rubric implementation

The repository now contains two applications:

1. **Original MediConnect website** at the repository root (React + TypeScript + Vite).
2. **Java Swing desktop application** in `java-gui/`, added specifically for the GUVI HCL Java GUI marking rubric.

Open `java-gui/README.md` for the full MySQL setup and run instructions.

## Rubric mapping
| GUVI criterion | Java implementation |
|---|---|
| OOP | `model/Person`, `Patient`, `Doctor`, `Admin`, `Payable`, `ConsultationBill`; custom exceptions |
| Collections & Generics | `Repository<T>`, `InMemoryRepository<T>`, `List`, `Map` |
| Multithreading & Synchronization | `AppointmentService` (`ExecutorService`, `Future`, `AtomicInteger`, synchronized methods/collection); SwingWorker |
| Classes for database operations | `PatientDAO`, `DoctorDAO`, `AppointmentDAO` |
| Database Connectivity (JDBC) | `db/Database` |
| Implement JDBC for database connectivity | DAO insert/read operations and `database/schema.sql` |

This is a learning/demo implementation. Configure and test it with your own MySQL installation before submitting. It is not a production system and must not contain real patient records.
