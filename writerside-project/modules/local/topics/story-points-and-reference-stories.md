
# Story Points & Reference Stories
This page contains an introduction to using Reference Stories for Estimation using story points and a set of reference stories for the team. 

Keep in mind, the goal of estimation is not to create perfectly accurate predictions, but rather to help the team plan their work and communicate effectively about it. Reference stories are a tool that can help achieve this goal.

The primary goal is to establish a shared understanding within the team of what each story point value represents. This will help in estimating the effort required for new user stories.

## Advantages of Story Points {collapsible="true"}
Estimating in story points instead of hours has several advantages:

1. **Focus on Complexity, Not Time**: Story points measure the complexity of a task, not the time it takes to complete. This is beneficial because different team members may take different amounts of time to complete the same task due to varying levels of experience and expertise.

2. **Accommodate for Uncertainty**: Story points allow for a degree of uncertainty. When tasks are estimated in hours, there can be an expectation of precision that is often unrealistic given the inherent uncertainties in software development.

3. **Promote Team Velocity**: Estimating in story points allows teams to measure their velocity, or how much work they can complete in a given time period. This can be a more useful metric for planning and forecasting than individual hours.

4. **Avoid False Precision**: Hours can give a false sense of precision. With story points, it's clear that estimates are just that - estimates.

5. **Better Long-Term Planning**: Story points can be more consistent across sprints and teams than hours, making them a better tool for long-term planning.

6. **Encourage Deeper Discussion**: When estimating in story points, teams are often encouraged to have deeper discussions about the complexity and risks of a story, leading to a better shared understanding of the work.


## Purpose of Reference Stories {collapsible="true"}
Reference stories are used during Scrum Refinement for several reasons:

1. **Shared Understanding**: Reference stories help the team to establish a shared understanding of the complexity and effort involved in completing different types of work. This is particularly useful for new teams or teams that have recently experienced changes in composition.

2. **Consistency in Estimation**: They provide a baseline for estimating the size of new user stories. This helps to ensure consistency in the team's estimates over time.

3. **Efficiency**: Reference stories can make the estimation process more efficient by reducing the amount of discussion needed for each new user story. If a new story is similar to a reference story, the team can quickly assign it a similar point value.

4. **Calibration**: They allow the team to recalibrate their estimates as they gain more experience. If the team finds that a reference story took more or less effort than expected, they can adjust their estimates for similar stories in the future.

5. **Communication**: Reference stories can also be a useful communication tool when discussing the project with stakeholders. They can help to give a tangible sense of what the team means by a 'point'.


## Example of Reference Stories {collapsible="true"}

1. **Story Point 1**: A simple task such as fixing a typo in the frontend service written in React and TypeScript. This could be a typo in a label or a button text.

```markdown
As a user, I want to see the correct spelling of 'Submit' on the form 
button so that it looks professional.
```

2. **Story Point 2**: A slightly more complex task, such as adding a new field to a form in the frontend and saving it to the database. This involves changes in the frontend only.

```markdown
As a user, I want to add my phone number to my profile so that I can 
be contacted more easily.
```

3. **Story Point 4**: Implementing a new API endpoint in the backend and integrating it with the frontend. This involves changes in both the frontend and the backend.

```markdown
As a user, I want to see a list of all my past orders so that I can 
track my purchase history.
```

4. **Story Point 8**: A more complex task, such as implementing a new feature that involves changes in multiple microservices and requires integration with external systems like Microsoft Graph API, Salesforce, DAWA, etc.

```markdown
As a user, I want to insert travel from, to, addresses when booking a 
meeting so travel time can be included in the booked meeting.
```

5. **Story Point 13**: A large task that involves significant changes to the system, such as adding a new microservice.

```markdown
As a developer, I want to add a new microservice for handling payment 
processing so that we can support seat based subscription models.
```

6. **Story Point 20**: A very large task that might involve architectural changes or significant efforts in multiple areas of the system.

```markdown
As a developer, I want to refactor our database schema to improve 
performance and maintainability.
```

7. **Story Point 40**: A huge task that will likely need to be broken down into smaller tasks. This could involve major changes to the system architecture or the implementation of a large and complex feature.

```markdown
As a developer, I want to migrate our monolithic application to a 
microservices architecture to improve scalability and maintainability.
```

8. **Story Point 100**: This is typically a massive task or project that will need to be broken down into multiple smaller tasks. It's often a sign that the task needs more analysis to be properly understood.

```markdown
As a business, we want to expand our product to a new market which 
will require significant changes to our system to support new 
regulations and languages.
```
