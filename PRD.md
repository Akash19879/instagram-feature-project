# Feature: Undo Send for Instagram DMs

## 1. Problem
Instagram users often send messages with typos, the wrong tone, or to the wrong person — especially in fast-paced chats. While users can delete a message after it’s sent, the recipient may already see it, causing confusion or embarrassment. There is currently no grace period to undo a message before it reaches the recipient.

## 2. Goal
To reduce accidental message sends by giving users a short, non-intrusive window to undo their last message — improving trust, user control, and overall DM experience.

## 3. Success Metrics
- At least 30% of eligible users use “Undo Send” within 2 weeks of launch  
- 30% reduction in message deletions within 30 seconds of sending  
- 15% increase in user satisfaction score for DMs (via in-app surveys)

## 4. User Stories
- As a casual user, I want to undo a message quickly so I can fix a mistake before the recipient reads it.  
- As a professional using Instagram DMs for work, I want to avoid sending messages to the wrong person.  
- As a teenager, I want to stop a message I regret sending to avoid embarrassment.

## 5. Requirements
- After sending a DM, a “Message Sent” confirmation with an “Undo” option appears.
- The “Undo” button remains active for 10 seconds.
- If “Undo” is clicked:
  - The message is not delivered to the recipient.
  - The message disappears from the sender's chat history.
- If no action is taken within 10 seconds:
  - The message is delivered normally.
  - The “Undo” option disappears automatically.
- Visual feedback (e.g., subtle countdown timer or disappearing toast notification)

## 6. Timeline
- Week 1: UX mockups and interaction flow  
- Weeks 2–3: Frontend and backend implementation  
- Week 4: QA testing and bug fixes  
- Week 5: Gradual rollout (10% → 50% → 100%)

## 7. Risks / Edge Cases
- Delay in message delivery may feel laggy or confusing to users  
- Users may expect the feature to work for all past messages, not just recent ones  
- Risk of misuse: users may try to manipulate the feature for unclear intent  
- Technical challenge: ensuring the message is suppressed in both sender and recipient chat logs
