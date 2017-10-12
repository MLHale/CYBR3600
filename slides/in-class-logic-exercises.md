# Logic Exercises
Imagine that you are a policy analyst and you are given the following natural language policies. 

## Exercise 1: PKI Computer System use policy
Convert the following into logic, then state a violation case.

### Policy Natural Language Text

***Acceptable Computer use in PKI***
- Users must have approved account credentials to log in to a system.
- Only students and faculty that work in or attend classes in PKI should have approved credentials.
- Authenticated users must not leave the systems they access unlocked and unattended when logged in. All systems should have an auto lock feature that locks the system after 5 minutes of inactivity when a user is authenticated. 

#### Tasks
Work as a group to:
- State the Policy using first-order logic
- Identify a single violation and state it formally

## Exercise 2: Student Account non-repudiation policy
Convert the following into logic, then state a violation case.

*** Student account non-repudiation and logging***
- All student account transactions must be logged and stored for 7 years.
- Transaction logs must include, at a minimum, the time when the transaction occured, the location and name of the on-campus vendor where the transaction occured, the total cost of the transaction, and the id of the point of sale system that the transaction occurred on. 

#### Tasks
Work as a group to:
- State the Policy using first-order logic
- Identify a single violation and state it formally

#### Hint 
This one is much harder than the first one. Note that you can nest quantifiers. Also be sure to properly quantify all variables.
