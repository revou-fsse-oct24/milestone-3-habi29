# UML Activity Diagrams

## Purpose of Each Diagram

### 1. User Authentication Activity Diagram
The **User Authentication** activity diagram visualizes the login process for users in the RevoBank system. It captures:
- The process of entering login credentials.
- Verification of credentials by the system.
- Handling of incorrect login attempts.
- Successful authentication leading to token generation.
- The final outcome, whether the login succeeds or fails.

### 2. Transaction Handling Activity Diagram
The **Transaction Handling** activity diagram represents the process of handling financial transactions in the RevoBank system. It details:
- How a user initiates a transaction.
- The verification of the account balance before proceeding.
- The transaction process if the balance is sufficient.
- Handling of failed transactions due to insufficient funds.
- The generation of transaction history for successful transactions.

---

## Key Decisions and Processes Represented

### User Authentication:
- **Decision:** Is the entered credential valid?
  - Yes → Generate token and log in.
  - No → Record failed attempt and send an email notification.
- **Process:** 
  - If valid, the system generates a token and grants access.
  - If invalid, the system records the failed login attempt and notifies the user.

### Transaction Handling:
- **Decision:** Does the user have sufficient funds?
  - Yes → Process the transaction and update transaction history.
  - No → Decline the transaction and notify the user.
- **Process:**
  - The user initiates the transaction, and the system verifies account balance.
  - If the balance is sufficient, the transaction is processed and recorded.
  - If insufficient, the transaction fails, and the user is notified.

---

## UML Activity Diagrams
The UML activity diagrams were created using **Lucidchart**:
- **User Authentication:** [Lucidchart Diagram](https://lucid.app/lucidchart/be18c548-70b9-439c-9e48-d4d57175da62/edit?viewport_loc=0%2C-1804%2C1479%2C721%2C0_0&invitationId=inv_e05df861-eefa-4cd6-a5c0-32f453a60aa1)
- **Transaction Handling:** [Lucidchart Diagram](https://lucid.app/lucidchart/44ea703b-e8a9-40ec-90e2-06f6db9fab0f/edit?viewport_loc=71%2C311%2C1479%2C721%2C0_0&invitationId=inv_25e7aabe-8608-4c78-b743-8d2424a873d2)