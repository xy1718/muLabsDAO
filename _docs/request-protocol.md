---
title: Request protocol
prev_section: proposals.html
next_section: decisions.html
---

The Request Protocol
====================

The Request protocol is a lightweight, decentralized issues routing protocol. It is designed to be the simplest possible way to handle requests or [proposals](proposals.html) that are shared by a distributed group of people. We use it mostly to handle incoming requests.

When a Request or a [Proposal](proposals.html) comes in it is warm, juicy and soft. If it sits around for a day it will get cold. If it sits around several days it will become dry and hard. You can warm up an old Request in the microwave oven as long as it hasn't become too dry.

So, a Request and [Proposal](proposals.html) should be eaten fairly quickly or thrown away. No use stuffing it in a box. If you can't eat it yourself, offer it to someone else - before it gets cold, dry and hard!

How the request protocol works
------------------------------

When a Request is born:

**A Request always has an owner** - the person who received the Request or [Proposal](proposals.html). Or more specifically, the person responsible for the communication channel through which the Request appeared. 

**When you have a Request, you are responsible for taking care of it before it gets too dry!** Preferably within 1 working day, definitely within 2.

You have 3 options when is an simple issue or request:

-   **Eat it yourself.** The Request is now consumed, i.e. it has found a home and will not be routed anywhere.
-   **Give it to somebody else.**  You can't push the Request to someone, you can only offer it. The receiver has to pull the Request from you.
-   **Throw it away.** when I don't need to know or care if that happens :o) 

The one thing you should NOT do is just let the Request sit and dry. Better to explicitly throw it away in that case (i.e. tell the sender that we can't help).

So initially a Requests appears through a "push" protocol, i.e. the initial recipient gets the Request whether he wants to or not. After that, however, everything is "pull"-based.

Remember that the [Proposals](proposals.html) must be shared always with everybody in a most structure way!

Summary of the rules
--------------------

-   **As receiver of a Request you are responsible** until it is eaten by you, taken by someone else, or thrown away. If several people are interested, sync with them.
-   **A Request should not get more than 1-2 days old** without being eaten by somebody, thrown away, or reheated (by talking to the customer/sender).
-   **You can't push a Request onto someone else, they have to pull**. The Request is yours until someone else explicitly takes it (for example by saying "I'll take the Request"). You can of course recommend (or even try to convince) someone else to take it from you. This goes both ways - if someone offers you a Request, you don't have to respond if you aren't interested.
-   When in doubt:
    -   Broadcast an email to everybody who might be interested or involved in this Request).
    -   or send the Request to "upwards" or to a central person such the board. 
-   **When broadcasting to find interested Request-takers, give your colleagues one day** to indicate interest in the Request. Don't just let the first one that answers have the Request. There might be more interested. Letting the first one that answers having the Request leads to race conditions and might cause tension between colleagues.

We don't always succeed in following these rules, especially the 1-2 day age limit. But we really try our best, and we're at least aware of when we fail.

Why it could works
------------------

-   **Simple**, anybody can learn it in 5 minutes.
-   **Can be extended** as needed. New rules can be added, tool support can be added. But don't. Keep it simple and add stuff only if you really, really need it.
-   **Doesn't require any specific artifacts** or documents that need to be maintained (unless you add that layer yourself...).
-   **Decentralized** - uses "wisdom of the crowds" to ensure that Requests reach the right destination in the shortest possible time with the least possible effort. People  can focus on important stuff and not become a bottleneck for all kinds of trivial requests.
-   **Customer focused** - customers normally get a response within a reasonable time.
-   It **promotes trust and collaboration**, and avoids bottlenecks and command & control
-   It is **Lean** - we minimize work in progress and maximize flow by ensuring that Requests are handled quickly and don't pile up in queues. We minimize waste and stress in the system by discarding sour Requests quickly.
-   We **still have the option to centralize & escalate** on a case-by-case basis. If someone bumps into a Request that needs to be escalated to some central authority then that can be done immediately.

FAQ
---

### Does this work for all types of requests?

We don't know. But it has worked well enough so far, and we haven't come up with any kind of request where it wouldn't work.

### What if several people want the same Request?

If several people are interested in the same Request, they talk to each other and sort it out.

Strictly speaking, the first person to take the Request has it, so in theory we have a race condition. In practice, however, when a potential conflict arises the involved people talk to each other (by phone or email) and decide on who should take the Request, based on who can serve the client best, who needs the Request most, and other relevant factors.

The [conflict handling process](conflict-handling.html) should help solve the edge cases.

### What if it is a critical request? Shouldn't some central authority handle it?

The closest thing we have to a central authority is the [board of trust](board-of-trust.html). If one of them received the request then, well, they already have it.

But don't forget - the Request is still yours until someone else explicitly takes it from you!

### What about traceability?

Traceability can be useful, for example we could write the Requests into a backlog or CRM system or something. That doesn't conflict with the Request protocol, we could just add that on top. But traceability has a cost. The overhead cost of each Request increases, due to writing & reading & updating information in a tool. So we don't really prioritize traceability.

### Won't a Request get dry if it gets sent around between people for too long?

Yes. So keep that in mind when you pass around Requests. Check the age, all emails have dates. Use common sense. If it is an urgent Request, it is getting old and you want to send to someone else, then call instead of sending email. 

### How do we avoid Requests falling through the cracks

Be very clear in your communication. Short, clear phrases like:

-   "Who will take this Request?"
-   "I'm taking the Request!"
-   "I will throw this Request away if nobody takes it by Tuesday"

We use the subject-line REQUEST for all Request-routing emails (see [email conventions](email-conventions.html)).

### What would be alternatives to the Request protocol?

Let's say something important comes in, such as a request from a new potential client. Some alternatives to the Request protocol would be:

-   **Alternative A: I can do whatever I want.** Perfectly fine to let the email sit unanswered in my inbox, or throw away the email without answering the client.
    -   **Result:** Lost business, disappointed customers, disappointed colleagues. My friend might have wanted that client, and I dumped it. Next time he'll dump a client that I would have wanted.
-   **Alternative B: All client requests have to be sent to person X** 
    -   **Result:**  becomes a bottleneck. And we miss the chance to utilize the collective intellect of the rest of the team.
-   **Alternative C: I have to be responsible for this request until it is completely resolved, I can't hand over to someone else.**
    -   **Result:** Stress and ineffectiveness, since I can't detach from a request that doesn't interest me. If I get a request that is more suitable for someone else, it is more effective for all parties if I connect the client with that person and eject myself from the loop.

Nah, we like the Request protocol better. It introduces a minimum amount of discipline and rules without becoming a burden.

### What are the potential disadvantages of the Request protocol?

-   Requires discipline and trust from everyone involved. But we kinda want that anyway...
-   No built-in traceability and visibility. We can't easily see which active Requests are in our system unless we add a visibility layer.
