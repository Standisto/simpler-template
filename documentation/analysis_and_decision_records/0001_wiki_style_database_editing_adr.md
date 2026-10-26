# ADR: wiki-style database editing

**Status:** Draft 

## Context and Problem Statement

We want to allow many people to collectively edit and contribute information stored in a database (like Airtable, Notion, or SQL). This will help us gather and maintain a single, shared source of truth for [Simpler Co-op](https://github.com/orgs/simpler-coop).

The goal is to enable many people to collectively work on gathering information and contributing it to a shared source of truth in a database. 

What this is NOT: This is *not* simply creating a Markdown file that contains a table of data. That approach will not meet our need for editing a database because it is ultimately store as plain-text, not database values.

## Decision Drivers

## Must have

The solution must satisfy the following needs to be successful:

1. **Database foundation:** The data must live in a proper database (e.g., Airtable, SQL, Notion). We cannot just edit data inside a simple text file.
2. **Individual accountability:** Every user must have an account so that we can track who made which change.
3. **Submit new entries:** Individual users must be able to submit new data to blank fields in the database.
4. **Edit existing entries:** Individual users must be able to edit data that already exists in fields in the database.
5. **Admin review gate:** Administrators must have the ability to review and approve all contributions before they are saved to the main database. The admin review gate should be an option that can be turned on or off. 
6. **Simple access:** Account creation must be easy and quick. We should reuse existing logins (like Google or GitHub accounts) to simplify this process.
7. **Easy user experience (UX):** The process for making edits must be very simple and easy to understand, even for people who are not technical. (For example, complex processes like submitting a "pull request" via GitHub are too complicated for our general users.)

## Nice to have 

These features improve the experience but are not mandatory for the solution to work:

1. **Common tooling:** The solution should primarily re-use common tools (such as Airtable, Google Sheets, or others) that are proven to be stable and reliable at scale. We want to avoid building complex, custom software that introduces new bugs.
2. **User management control:** Admins should have the option to completely remove or ignore all edits made by a specific user (e.g., if a user is determined to be spamming or unreliable).
3. **Live Co-Editing:** Users should be able to see changes made by other users in real-time as they are happening.

## Not necessary

1. **Structural Changes:** It is not necessary for regular users to be able to change the fundamental structure of the database (e.g., adding new tables or columns). Only administrators should have permission to make these structural changes.

## Options Considered

* {option 1}  
* {option 2}  
* ...

## Decision Outcome

Chosen option: "{option 1}", because {justification. e.g., only option which meets a key decision driver \| which satisfies x condition \| ... }.

### Positive Consequences

* {e.g., improved performance on quality metric, new capability enabled, ...}  
* ...

### Negative Consequences

* {e.g., decreased performance on quality metric, risk, follow-up decisions required, ...}  
* ...

## Pros and Cons of the Options

### {option 1}

{example \| description \| pointer to more information \| ...}

* **Pros**  
  * Good, because {argument a}  
  * Good, because {argument b}  
  * ...  
* **Cons**  
  * Bad, because {argument c}  
  * ...

### {option 2}

{example \| description \| pointer to more information \| ...}

* **Pros**  
  * Good, because {argument a}  
  * Good, because {argument b}  
  * ...  
* **Cons**  
  * Bad, because {argument c}  
  * ...

## Links

* \[{Link name}\](link to external resource)  
* ...

