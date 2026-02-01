Coach/Admin
-
  - As a coach, I want to be able to create events with location, start time, duration so other team members can plan ahead
    - Acceptance: required fields are validated; events appear in team schedule; members can view event as soon as is made; there is a event title and timezone.
  - As a coach, I want to be able to edit events information, so changes can be viewed by team
    - Acceptance: saved with "last updated" time stamp; members see updated details; notify on change of time/date/location/status/deadline changes.
  - As a coach, I want to be able to cancel events with a reason so team members are aware why
    - Acceptance: status of event = "cancelled"; reason is visible; members are notified; RSVP is closed; event is visible but greyed out and not accessible.
  - As a coach, I want to add RSVP deadlines so attendance is confirmed by a specific time
    - Acceptance: team members can do "late RSVP" if they RSVP after deadline; deadline is viewable in UI
  - As a coach, I want to be able to see RSVP counts and member status so I can plan session
    - Acceptance: have a count of Going/Maybe/Late by "n" input time/Not Going/No Response / Either response but late; list view by response with team members and their response.
  - As a coach, I want to be able to sned connect requests to a player or parent using their email
    - Acceptance: coach enters email and selects player/parent role; request is created with status "Pending"; team member gets email notification; coach can cancel pending request; request expires after 7 days; once accepted member has access immediately; removing member revokes access at that moment
  - As a coach, I want to add links and documents to a team resources section so key info is centralized
    - Acceptance: links and documents are saved into their own section; only team members that have access to that team can access/view those resources


Parent
-
  - As a parent, I want to link my child to my account if they have one and can link to multiple children.
    - Acceptance: parent is able to link to player account or create a "child profile"; coach sees parent/player relationship
  - As a parent, I want to accept a connect request on behalf on my child so it can be linked and added to the team
    - Acceptance: parents accepts the request and joins the team; if parent and child are linked then parent can accept on behalf of both; parent-child relationship can be seen by coach even if parent is not added;
  - As a parent,I can see multiple teams if I am linked to 2 of my children that are on 2 different teams.
    - Acceptance: parent is able to toggle between teams of children; No toggle option if both children play on the same team.
  - As a parent, I want to RSVP for my child so the coach is aware of their attendance
    - Acceptance: parent response is saved; RSVP is recorded for the child, set by parent (source=parent); RSVP is before deadline

Player
-
  - As a player, I want to accept or decline team connect request so I can join team without having to search for team
    - Acceptance: player cannot find teams, player sees list of connect requests "Pending"; if accepted player is added; if declined request disappears; expired requests disappear; matching account to connect request should receive invite only

Team Member (Parent or Player)(shared)
-
  - As a team member, I want to be able to sign up in app
    - Acceptance: user can sign up with email & password or SSO, after sign-in user sees empty team if not yet joined one; authentication errors are shown clearly (invalid password)
  - As a team member, I want to be able to see and respond Connect request from team so I can join it
    - Acceptance: notification in email about invite; request is viewable in app in "Requests" tab; accepting request adds access to team events and resources immediately, declining eliminates request and does not give access; connection requests are unique (resending updates existing)
  - As a team member, I want to view the team schedule so I can plan ahead for events
    - Acceptance: events are viewable by calendar or list; event information (time, location, duration, etc) must be available; event status if cancelled must be available
  - As a team member, I want to RSVP to events so attendance is available to the coach
    - Acceptance: possible to RSVP before deadline, response is saved (Yes, Maybe, No, No response - if nothing said by deadline
  - As a team member, I want to receive notifications for cancellations or changes in events so I am up to date
    - Acceptance: when event is cancelled I will receive a notification and will grey out event + not allowing for RSVP; when event is changed there will be a notification saying information changed
  - As a team member, I want to receive a reminder 2 hours before RSVP deadline time so I can make sure I respond on time
    - Acceptance: 2 hours before the deadline team member will receive email notification; notification is not sent if already RSVP'd
