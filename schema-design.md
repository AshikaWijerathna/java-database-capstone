## MySQL Database Design

Table: patients

id: INT, Primary Key, Auto Increment
full_name: VARCHAR(100), Not Null
email: VARCHAR(100), Unique, Not Null
phone: VARCHAR(20), Not Null
date_of_birth:DATE
gender:VARCHAR(20)
address: VARCHAR(255)

Table : doctors
id:INT, PRimary Key, Auto Increment
full_name: VARCHAR(100), Not Null
email: VARCHAR(100), Unique, Not Null
phone: VARCHAR(20), Not Null
specialization: VARCHAR(100), Not Null
clinic_location_id: INT, FOREIGN Key -> clinic_locations(id)

Table : appointments
id: INT, Primary Key, Auto Increment
doctor_id: INT, Foreign Key -> doctors(id)
patient_id: INT, Foreign Key -> patients(id)
appointment_time: DATETIME, Not Null
status: INT, Not Null
0 = Scheduled
1 = Completed
2 = Cancelled
reason: VARCHAR(255)

Table : admin
id: INT, PRimary Key, Auto Increment
username: VARCHAR(50), Unique, Not Null
email:VARCHAR(100), Unique, Not Null
password_hash: Varchar(255), Not Null
role: VARCHAR(50), Not Null

Table: clinic_locations
id:INT, PRimary Key, Auto Increment
name:VARCHAR(100), Not Null
address; VARCHAR(255), Not Null
phone: VARCHAR(20)

Table: payments
id:INT, Primary Key, Auto Increment
appointment_id: INT, Foreign Key -> appointments(id)
amount:DECIMAL(10,2), Not Null
payment_method; VARCHAR(50), Not Null
payment_status:INT, Not Null
0 = Pending
1 = Paid
2 = Failed
paid_at:DATETIME

Table : doctor_availability
id:INT, Primary Key, Auto Increment
doctor_idINT, Foreign Key -> doctors(id)
available_date:DATE, Not Null
start_time:TIME, Not Null
end_time:TIME, Not Null
is_available:BOOLEAN, Not Null

Table : prescriptions
id: INT, Primary Key, Auto Increment
appointment_id: INT, Foreign Key -> appointments(id)
medicine_ name: VARCHAR(100), Not Null
dosage:VARCHAR(100), Not Null
instructions: VARCHAR(255)
issued_date:DATE, Not Null

## MongoDB Collection Design

Collection: messages
### Collection: messages
{
  "_id": "ObjectId('64abc123456def789')",
  "appointmentId": 51,
  "patientId": 12,
  "doctorId": 7,
  "conversationType": "appointment_followup",
  "messages": [
    {
      "senderRole": "patient",
      "senderId": 12,
      "message": "Doctor, should I continue this medicine if I feel better?",
      "sentAt": "2026-05-28T10:30:00Z",
      "read": true
    },
    {
      "senderRole": "doctor",
      "senderId": 7,
      "message": "Please complete the full course as prescribed.",
      "sentAt": "2026-05-28T10:45:00Z",
      "read": false
    }
  ],
  "tags": ["follow-up", "medicine", "non-urgent"],
  "metadata": {
    "createdBy": "patient",
    "priority": "normal",
    "source": "patient_portal",
    "lastUpdated": "2026-05-28T10:45:00Z"
  },
  "schemaVersion": 1
}




