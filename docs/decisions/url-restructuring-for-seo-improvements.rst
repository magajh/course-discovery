23. URL Restructuring for SEO Improvements (Updated URL slug pattern)
=====================================================================

Status
=======

Accepted (June 2023)

Context
=======
There exists a default breadcrumbing structure for Open Courses in Discovery that auto generated course slugs based on course_title
which define the marketing URL path on the website `edx.org`.The existing URL structuring doesn't provide Google an SEO friendly sitemap for indexing and doesn't reflect branding tone and voice. 
As part of structuring all course About Pages will be tied to the most relevant Learn Page - existing or newly created on www.edx.org. The goal of this url_slug update is the improved 
SERPs and indexing by Google.

Decision
=======
To Improve SERPs and indexing by Google, the URL slug pattern for the courses will be updated.
The current URL slug pattern for the courses is generated from the course title. Rather than generating slug from course title now slug will be created using course title, primary subject and organization.
For OCM courses, the slug will be updated to `learn/{primary_subject}/{organization_name}/{course_title}`. The `/course/url-slug` will be deprecated.
For Bootcamps & execEd the format is `/boot-camp/<org-slug>-<title-slug>` & `/executive-education/<org-slug>-<title-slug>` respectively.
The updation of slugs will be done in the phases. The first phase will be to update the slugs for OCM courses.
The subsequent iterations, depending upon the results of OCM updates, will take care of Bootcamp, ExecEd, and Programs.
