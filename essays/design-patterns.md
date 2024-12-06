---
layout: essay
type: essay
title: "The World of Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2024-12-05
published: true
labels:
  - Design Patterns
  - Typescript
  - React
---

<img class="img-fluid" src="../img/design/design-header.png">

# Constructing the groundwork of a successful application

If you had to imagine that you were standing at a construction site and managing your workers, how would you even start building something substantial? If you had to build a tall skyscraper or even a small home, you would first need to have one of the most crucial things: a blueprint. The blueprint is a guide; a set of proven structures and techniques to ensure that all the rooms, walls, and windows come together in a flawless design. Without having a blueprint, the building won't come to fruition, and it'll likely be a mess once it's finished. Instead of inventing the wheel from scratch, we use the blueprint to use previously successful design tips to execute the creation of the building with less errors, less mess, and a higher success rate.

This analogy doesn't just only describe a blueprint for a construction project, but it also applies to design patterns in software engineering. Design patterns are almost like an architect's blueprint. The design patterns offer reusable templates that guide us developers in building reliable, efficient, and highly scalable code.

The history of the design pattern comes from the "Gang of Four" book, released in 1994 that talked about design patterns in a way that related to software engineering. In the book, it mentioned the reusability of code, and the true tried and tested ways that developers wrote and designed code. 

# The personal use of design patterns in my own code

In my code, I remember using the Decorator Pattern. The Decorator Pattern is a structural desgin pattern that allows behavior to be dynamically added to objects without modifying the original code. In simpler terms, you typically have a core object or function, and that function is wrapped with additional functionality that extends or modifies the behavior of the original function. In the ICS314 final project, I implemented Yup validation which mimicks this design pattern. Yup validation was used everywhere in our code but I recall using it most when creating the function to edit activities.

In our EditActivityForm.tsx file, here is the onSubmit function:

```
const onSubmit = async (data: Activity) => {
  // console.log(`onSubmit data: ${JSON.stringify(data, null, 2)}`);
  const cleanedData = {
    ...data,
    registered: data.registered.filter((user) => user.trim() !== ''),
  };
  await editActivity(cleanedData);
  swal('Success', 'The activity has been updated', 'success', {
    timer: 2000,
  });
};
```

This function takes in the data (as type Activity) and first cleans it. The cleaning is done by taking the 'registered' portion of the data and removing any empty strings in the 'registered' array. Then, before the editActivity(cleanedData) function is called, a simple line must be true:

```
resolver: yupResolver(EditActivitySchema),
```

This resolver checks (using Yup) to see if the data matches our validation schema, which is shown below:

```
export const EditActivitySchema = Yup.object({
  id: Yup.number().required(),
  name: Yup.string().required(),
  description: Yup.string().required(),
  location: Yup.string().required(),
  date: Yup.string().required(),
  time: Yup.string().required(),
  author: Yup.string().required(),
  author_email: Yup.string().required(),
  duration: Yup.number().positive().required(),
  registered: Yup.array().required(),
});
```

This essentially validates if all the data in the form is correct. The .required() fields must be fulfilled, and other stuff like .number() and .string() make sure that the data types are correct. This example in our final project illustrate the decorator design pattern since it adds validation logic, which happens externally and doesn't change the original form component.