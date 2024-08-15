# Guvi Zen Class Database Model

## Entities:

1. **Students**
2. **Instructors**
3. **Courses**
4. **Enrollments**

## Attributes:

- **Students**: `student_id`, `first_name`, `last_name`, `email`, `phone_number`, `date_of_birth`
- **Instructors**: `instructor_id`, `first_name`, `last_name`, `email`, `expertise`
- **Courses**: `course_id`, `course_name`, `description`, `start_date`, `end_date`, `instructor_id`
- **Enrollments**: `enrollment_id`, `student_id`, `course_id`, `enrollment_date`

## Relationships:

- **One-to-Many**:
  - One Instructor can teach multiple Courses.
  - One Course can have multiple Students.
- **Many-to-Many**:
  - Students can enroll in multiple Courses and a Course can have multiple Students. This is represented by the Enrollments table.

## Schema Description:

This database model is designed to manage the data of a Guvi Zen class, including students, instructors, courses, and enrollments. The relationships between these entities are established using foreign keys, ensuring data integrity and efficient querying.
