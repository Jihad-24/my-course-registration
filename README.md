# Course-Registration

Click here for the live link: [https://course-registration-react.netlify.app/]

- Some Features of the  Project

# 1. Course Selection : 
  - Users can see a list of available courses displayed as cards. They can view details such as course title, description, price, and credit hours. By clicking the "Select" button on a course card, users can add that course to their selection.

# 2. Credit Management : 
  - The project has a credit management system. Each selected course consumes a certain number of credit hours, and the total credits used and remaining credits are displayed to the user. If a user tries to select a course that would exceed their available credit, they receive an error message.

# 3. Shopping Cart : 
  - The project has a shopping cart component (imported from Cart.js) that displays the courses the user has selected. It shows the total price of the selected courses, the remaining credits, and the total credits used. Users can see the details of their course selection and manage their choices within the cart.

- Discuss how you managed the state in your assignment project.

# Declaring State : 
  - Multiple state variables are declared using the useState hook. These variables are used to store different pieces of information related to the course registration.

- allCards : Stores an array of all available courses.
- selectedCard : Stores an array of courses selected by the user.
- totalRemaining : Stores the remaining credit hours available to the user.
- totalCredit : Stores the total credit hours used by the selected courses.
- totalPrice : Stores the total price of the selected courses.

# Updating State : 
  - State variables are updated using the corresponding setter functions. For example, when a user selects a course, the state is updated in the handleSelectorcards function.There, setTotalCredit, setTotalRemaining, setSelectedCard, and setTotalPrice are used to update the state variables based on the user's actions.

# Using State in the Component : 
  - The state variables are used within the component to display information to the user and control the application's behavior. For example, the selectedCard state is passed as a prop to the ( Cart ) component to display the selected courses in the shopping cart.