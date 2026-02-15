# Exercise 2: Data Extraction Template

**Objective: Extract structured data from unstructured input.**

Choose an unstructured text (e.g., "John Doe, age 29, lives in Paris and works as a software engineer.").

Create a template prompt:

"Extract the following fields from the text: Name, Age, Location, Occupation. Return the output in JSON format."

Validate the output and ensure consistency across multiple inputs.

---
**The first prompt I gave it:**

Sam Smith, age 29, lives in Paris and works as a software engineer. Extract the following fields from the text: Name, Age, Location, Occupation. Return the output in JSON format.

**It's response:**
```json
    {
  "Name": "Sam Smith",
  "Age": 29,
  "Location": "Paris",
  "Occupation": "Software Engineer"
}
```

---
---

**The second prompt I gave it:**

Chisom Nnamani is a 25-year-old fashion designer who lives in Switzerland. She is originally from Nigeria, and loves playing Table tennis. She studied fashion and designing in Fashion Institute in India, and is married to Tom Cruise, with two healthy children.

Extract the following fields from the text: Name, Age, Location, Occupation, Country of Origin, Hobby, Alma Mater, and Husband's name.  Return the output in JSON format.

**It's response:**
```json
{
  "Name": "Chisom Nnamani",
  "Age": 25,
  "Location": "Switzerland",
  "Occupation": "Fashion Designer",
  "Country of Origin": "Nigeria",
  "Hobby": "Table Tennis",
  "Alma Mater": "Fashion Institute in India",
  "Husband's Name": "Tom Cruise"
}
```