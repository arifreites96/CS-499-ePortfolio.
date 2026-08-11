# Algorithms and Data Structures

[← Back to Home](index.md)

## Travlr Getaways

### Enhancement Two: Algorithms and Data Structures

#### Artifact Description

The artifact selected for the Algorithms and Data Structures enhancement is the Travlr Getaways full-stack travel application that I originally developed in CS 465: Full Stack Development I.

I selected this artifact because it provided an opportunity to improve how travel data was organized, processed, and displayed. In the earlier implementation, individual travel packages were written directly into the page structure. Although this approach worked with a small number of trips, it required repeated markup and would become more difficult to maintain as additional travel packages were added.

## Justification for Inclusion

For this enhancement, I redesigned the way trip information is stored and processed. Instead of hard-coding each travel package into the Handlebars template, I created a JSON file containing an array of trip objects.

Each object stores information associated with a travel package, including its name, image, description, length, start date, and price.

The application reads the JSON data and parses it into a JavaScript data structure. The resulting collection is passed from the controller to the Handlebars view, where the application iterates through the trip collection and dynamically generates the appropriate content for each travel package.

This enhancement demonstrates my ability to select and use an appropriate data structure for a computing problem. An array of structured objects is appropriate for the travel packages because each trip follows the same data model and the collection can be processed sequentially when the travel page is generated.

The enhancement also eliminates repeated HTML code. Previously, adding another travel package required manually creating another section of markup. With the enhanced implementation, additional trip objects can be added to the data collection and processed through the same rendering logic.

## Skills Demonstrated

Through this enhancement, I demonstrated skills involving:

- Data structures
- Algorithmic processing
- JavaScript
- JSON data handling
- Iteration
- Dynamic web application development
- Reusable application logic
- Separation of data from presentation

I also demonstrated the ability to evaluate an existing solution and replace repetitive implementation with a reusable algorithm.

## Course Outcomes

This enhancement primarily supports the following Computer Science program outcomes:

- Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.
- Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for implementing computer solutions that deliver value and accomplish industry-specific goals.

The enhancement demonstrates these outcomes through the use of structured data and reusable iteration logic instead of repeated hard-coded content.

## Reflection

Completing this enhancement helped me better understand that algorithms and data structures are not limited to complex mathematical problems. They also influence how everyday application data is organized, accessed, processed, and presented.

One of the most important things I learned was the value of separating data from presentation. In the original implementation, trip information and the HTML used to display it were closely connected. This meant that every new travel package required additional markup.

By moving the travel information into a structured collection and creating one reusable process to render the collection, the application became easier to understand and maintain.

One challenge during this enhancement was ensuring that the properties in the JSON objects aligned correctly with the properties referenced by the Handlebars template. Because the view depends on the structure of each object, inconsistent field names or missing data can prevent information from displaying correctly.

This reinforced the importance of maintaining consistent data structures throughout an application.

The enhancement also helped me recognize the trade-off between simplicity and scalability. Hard-coded data can be sufficient for a very small static website, but it becomes inefficient to maintain when the amount of information increases.

Overall, this enhancement demonstrates growth in my ability to organize application data, implement reusable processing logic, evaluate design alternatives, and build applications that can be expanded more efficiently.

---

[← Return to ePortfolio Home](index.md)
