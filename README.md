# notes

## frontend

**Question 1**

* why use react over other frameworks? advantages/disadvantages?

<details><summary>**Answer**</summary><p>

React is well known for its ease of use, reusability, and modularity as your code base grows.   
**PROS**
- Create reusable UI components
- Easy to learn; It combines the use of HTML and Javascript
- Efficiency when updating the UI. Compared to updating the whole web page (all the components) it updates specific components that trigger when needed.
- High Performance - allows for fast and reposive UI

**CONS**
- Focuses on View more in Model-View-Controller (MVC) pattern. Model and Controller aspect must be integrated with additional tools.
- JSX learning curve
- Fast-paced development may make it hard to keep learning all the new tools with each update.

</p></details>

**Question 2**

* why use redux? when to use it / when not to use it?

<details><summary>**Answer**</summary><p>
across compoments.

Redux is a useful state management tool that makes it easier to mangage the state of your application with the ease of accessing and updating the state globally vs. locally for each component.  This removes the complications of passing the state up and down between compoments. 

*When to use it?*
- A good amount of data is being passed between components.
- If you have difficulty detecting/tracing changes to the state.

*When not to use it?*
- Barely any data is not being passed between components.
- If you already have a predefined way of sharing and arranging the state

</p></details>
