# Process

## Scheduling and project management

#### 🔄 Cycles

Our team works in 3-week cycles. Each week starts on Monday.

The first two weeks of each cycle are focused on writing code. The third week is focused on deployment, feedback among the team, and planning the next cycle.

#### 🕴 Standups

We hold standups over Slack every Monday, Wednesday, and Friday at 8pm Pacific time.

Team members are expected to reply to the standup thread within twenty-four hours, so that everyone stays in sync.

#### 🗣 Check-ins

Since we all work different hours, it's team tradition to post a message in Slack when you come online, for example:

> Hi everyone! I'm going to be working on the frontend until about 4PM.

This is done in order to encourage collaboration at times that multiple people are working on the same thing simultaneously.

#### 🐞 Issue tracking

Features, improvements, bugs, and housekeeping tasks are tracked as cards on the [HRX Portal Trello board](https://trello.com/b/90MizePd/hrx-portal).

Team members should ensure that their current tasks are on the board, and that they've "joined" cards they're working on.

Anyone is welcome to create a new card, as long as a good description is provided so that others can understand it.

Below are some templates for descriptions, adapted from [Writing Better User Stories and Bug Tickets](https://medium.com/@Carmichaelize/writing-better-user-stories-and-bug-tickets-3cb5165e7db).

##### Feature/improvement cards

The goal here is to communicate _what_ the feature should do, _who_ benefits from it and _how_ they benefit. 

Acceptance criteria should generally lean towards describing functionality instead of implementation details, and should be clear enough that an implementer knows what their "finish line" is.

```
Title: "[Feature] Audible message notifications"

As a user, I want to hear sound alerts when sending and receiving messages so that conversations feel more immediate (and asynchronous).

### Acceptance criteria

- A notification is heard when a message is sent.
- A notification is heard when a message is received.
- A user should be able to enable/disable notifications in their Settings.

### Additional context or thoughts

We may want to create our own notification sound, since system default sounds may already be in use by other applications on the user's device.

This is out of scope for this now, but we may want to implement this in a way that allows us to build visible notifications on top of audible ones in the future, since deaf people and folks that keep their volume muted alike may want a way to be aware of new messages.

```

##### Bug cards

```
Title: "[Bug] Agent filters result in page redirect"

Users should be able to select (and apply) the ‘disabled’ filter on the ‘Agents’ page without being redirected to another page.

### To reproduce the issue...

- Log in and navigate to 'Agents' section.
- Select the ‘disabled’ filter button.

### Expected result

The agents table should only show ‘disabled’ agents.

### Actual result

The user is redirected to another page... an undefined ‘Agent’ page.

### Additional context or thoughts

It's possible this was implemented on purpose somehow, to keep data up to date... Therefore, care should be taken to make sure that the Agents data updates correctly when the redirect behavior is removed.
```

## Workflows and procedures

#### 👀 Code review

Each pull request opened against `master` must receive one approving review before being merged.

When a team lead reviews a pull request, they should do their best to provide high-level feedback about the architecture and approach of the code in question, as well as context around the change requests they make.

## Expectations

Each participant has given a 5 hour per week commitment to the team. 

Generally this is taken at face value, but if team leaders feel that a member isn't delivering on their commitment, action may be taken to preserve team morale.
