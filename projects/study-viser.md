---
layout: project
type: project
image: img/project_images/studyviserlogo.png
title: "Study-viser"
date: 2026
published: truee
labels:
  - Typescript
  - Next.js
  - Prisma
  - Vercel
  - GitHub
summary: "A responsive web application for UH courses that my team developed in ICS 314."
---

<img class="img-fluid" src="../img/project_images/study-viser_homepage.png">

Study-viser is a web application that I helped create as a team project in ICS 314, Spring 2026. The goal was to create a website in which teachers can assign terms, which their students would then submit definitions for, as a form of studying and perhaps extra credit. Students would also be able to use the terms submitted across all courses as a study guide. This project helped me to build a greater understanding of full-stack development.

For the front-end of the website we used Typescript, Next.js, and CSS. The back-end was built with Prisma, and the app was deployed with Vercel.

I was mainly in charge of the backend so I gained more experience with Prisma specifically. Here is an example of one of the Prisma models I created:
```
model Course {
  crn          Int       @id
  code         String  // if listing is set, should match listing.code
  secret       String    @unique @default(cuid()) // given to students to enroll
  title        String
  description  String?
  createdAt    DateTime  @default(now())
  updatedAt    DateTime  @updatedAt
  instructor   User?     @relation("InstructorCourses", fields: [instructorId], references: [id])
  instructorId String?
  listing      Listing?  @relation(fields: [listingId], references: [code])
  listingId    String?
  externalURLs String[]  // list of external study sources, specific to course
  location     String?   // optional until set by instructor
  students     User[]    @relation("StudentCourses")
  terms        Term[]

  @@map("courses")
}
```
In this application I imported every course listing for the Spring 2026 semester at UH Manoa then tied that listing to a specific course instance(the model is shown above), differentiated by its CRN. I also added CRUD (create, read, update, and delete) functions to the codebase for the models I created.

Over the course of a month my team and I worked on various issues and used GitHub to coordinate and assign tasks. Though GitHub has its share of problems, I found it integral in combining our various bits of code. [Study-viser Project page](https://study-viser.github.io/)
